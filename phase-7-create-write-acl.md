# Phase 7: Create the Write ACL

## Steps
1. Open **System Security > Access Control (ACL)** and click **New**.
2. Configure:
   - Type: `record`
   - Operation: `write`
   - Name: `u_institution_details`
   - Active: `true`
3. In the **Requires role** related list, add `bb3`.
4. Do not add a data condition, as specified in the project PDF.
5. Save the ACL.
6. Test with a user assigned `bb1`, `bb2` and `bb3`; verify that the user can view and edit EEE-branch records and has the New button available, as described in the PDF.

## Video narration
"I add a Write ACL requiring bb3. Then I test the user who has bb1, bb2 and bb3 to check whether editing is allowed."

## Result
The Write ACL is saved and edit access is ready for verification.
