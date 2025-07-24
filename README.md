
# Q\&A Submission Portal

This is a simple HTML web application for uploading question-and-answer files associated with course materials. Files are uploaded to Firebase Storage, and submission metadata is stored in Firestore. After a successful submission, the user is redirected to the most recent files.

* All file fields are required. Submission will fail if any field is left empty.
* The email field is used to organize files in Firebase Storage.
* You must replace `"https://docs.google.com/document/d/SHARED_DOC_ID/view"` with your actual shared document link in the HTML (`window.location.href`).

## File Structure

```
submissions/
  └── user@example.com/
        ├── lecture_717-filename.ext
        ├── welch_722-filename.ext
        └── ...
```
