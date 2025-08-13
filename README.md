Steps to create a repository on GitHub:

1. Log in to GitHub at [https://github.com](https://github.com).
2. Click the "+" icon in the top-right corner.
3. Select "New repository".
4. Enter a repository name (e.g., `file-organizer`).
5. Optionally add a description.
6. Choose visibility: Public or Private.
7. (Optional) Check "Add a README file", select a .gitignore (Python if needed), and choose a license.
8. Click the green "Create repository" button.
9. To add files using the website:

   * Go to the repository page.
   * Click "Add file" → "Upload files".
   * Drag and drop files, then commit changes.
10. Your repository is now ready and accessible on GitHub.

-------------------------------------------------------------------------------------------------------
This script’s idea is simple: it automatically organizes your files into folders based on their file type (extension).

Concept:

* Problem: Many folders (like your Downloads folder) get messy with different file types all mixed together — documents, images, videos, etc.
* Goal: Automatically separate files into folders so each file type has its own place.
  Example:

  ```
  Downloads/
      PDF_Files/
      JPG_Files/
      MP4_Files/
      no_extension_Files/
  ```

How it works step-by-step:

1. Get the folder path from the user (or hardcode it in the script).
2. Loop through all items in that folder.
3. Check if the item is a file (not a folder).
4. Extract the file’s extension (like .pdf, .jpg, .mp4).
5. If there’s no extension, label it "no\_extension".
6. Create a new folder named `<EXTENSION>_Files` (e.g., `PDF_Files`).
7. Move the file into that folder.
8. Repeat for all files.

Result:
Your folder becomes clean and organized, with files grouped by type.
