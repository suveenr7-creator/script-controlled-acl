# Phase 5: Test Read Access

## Steps
1. Impersonate the **EEE User** account and open the `u_institution_details` list.
2. Use the table list route `u_institution_details.list` in the All menu if needed.
3. Check which records are visible.
4. Test with a user who does not have the required role.
5. Impersonate an administrator and open the same list.
6. Compare the results with the verification points in the PDF:
   - A user with `bb1` should be able to view EEE-branch records.
   - A user without the role should not be able to view records.
   - An administrator should be able to view records across branches.

## Video narration
"Now I test the Read ACL with the EEE user, a user without the role, and an administrator. I compare each result with the verification criteria in the project document."

## Result
Read access has been tested for the role-based user, a user without the role, and an administrator.

**Note:** The PDF's script checks for `bb1`, while the data condition is Branch is EEE. If the actual instance does not filter records as expected, review how the ACL data condition and script are evaluated.
