UPLOAD INSTRUCTIONS (your site deploys through Vercel from GitHub)

1. Unzip this file on your computer. You will get a folder called "tools"
   containing: index.html, an "images" folder, and a "downloads" folder.

2. In GitHub, open your repository (cemmaikehi-dev/emmanuelikehi), on the "main" branch.

3. FIRST CLEAN UP the misplaced files in the top level (click each file,
   click the three dots menu at top right, choose "Delete file", then Commit):
     - index (6).html
     - book-cover.jpg
     - Blank_Sheet_Operator_Calculators.xlsx
     - Blank_Sheet_Operator_Toolkit.docx
     - Blank_Sheet_Operator_Toolkit.pdf
     - INDEX_EDITS.md
   KEEP: index.html (your homepage), IMG_20240318_161147_184.jpg (your About photo),
   and any CNAME or vercel.json file.

4. Click "Add file", then "Upload files". Drag the WHOLE "tools" FOLDER
   (not the files inside it) into the box. Chrome and Edge keep the folder structure.
   You should see paths like tools/index.html and tools/downloads/... listed.
   Commit changes.

5. Wait about one minute for Vercel to redeploy, then test:
     https://www.emmanuelikehi.com/tools/
     https://www.emmanuelikehi.com/tools          (no slash)
     https://www.emmanuelikehi.com/#book          (cover should now show)
   and click each Download button.

Final structure in GitHub:
  index.html
  IMG_20240318_161147_184.jpg
  tools/
    index.html
    images/book-cover.jpg
    downloads/Blank_Sheet_Operator_Toolkit.pdf
    downloads/Blank_Sheet_Operator_Toolkit.docx
    downloads/Blank_Sheet_Operator_Calculators.xlsx
