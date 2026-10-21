# Phase 2: Create the Institution Details Table

**Navigation:** All > System Definition > Tables > New

## Steps
1. Create a custom table with:
   - Label: **Institution Details**
   - Name: `u_institution_details`
   - Extends table: **false** (as specified in the project PDF)
2. Click **Submit**.
3. Add these fields to the table:
   - Student Roll Number — Auto Number
   - Student Name — Reference: User
   - Faculty Name — Reference: User
   - Branch — Choice: `ECE`, `EEE`, `CSE`
   - Email — String
   - Phone Number — String
   - Description — Multi String
4. Save the table and verify the fields are present.

## Video narration
"Next, I create the Institution Details table and add the student, faculty, branch and contact fields listed in the project document."

## Result
The `u_institution_details` table is ready to store institution records.
