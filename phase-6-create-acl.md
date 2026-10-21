# Phase 6: Create the Create ACL

## Steps
1. In **System Security > Access Control (ACL)**, click **New**.
2. Configure:
   - Type: `record`
   - Operation: `create`
   - Name: `u_institution_details`
   - Active: `true`
3. In the **Requires role** related list, add `bb2`.
4. Do not add a data condition, as specified in the project PDF.
5. Save the ACL.
6. Test the New button with a user who has `bb1` and `bb2`, and confirm the expected access.

## Video narration
"Next, I create the Create ACL for Institution Details. This ACL requires bb2 and does not use a data condition, following the project instructions."

## Result
The Create ACL is saved and the New-button behavior can be tested.
