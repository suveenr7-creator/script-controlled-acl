# Phase 4: Create the Read ACL

**Navigation:** All > System Security > Access Control (ACL)

## Steps
1. Open Access Control (ACL). Elevate the **security_admin** role if prompted or required.
2. Click **New** and configure the ACL:
   - Type: `record`
   - Operation: `read`
   - Name: `u_institution_details`
   - Active: `true`
   - Advanced: `true`
3. In the **Requires role** related list, add the custom role `bb1`.
4. Add the data condition **Branch is EEE**, as specified in the project PDF.
5. In the Script field, enter:

   ```javascript
   (function () {
       // Allow admin users full access
       if (gs.hasRole('admin')) {
           return true;
       }

       // Allow users with bb1 to pass this script check
       if (gs.hasRole('bb1')) {
           return true;
       }

       // Deny access for all others
       return false;
   })();
   ```

6. Submit the ACL.

## Video narration
"I create a record-level Read ACL for Institution Details. It requires role bb1, includes the Branch is EEE data condition, and uses the script shown in the project document."

## Result
The Read ACL is saved for `u_institution_details`.
