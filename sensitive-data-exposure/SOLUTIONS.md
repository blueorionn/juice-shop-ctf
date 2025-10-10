# SOLUTIONS

## 1.Confidential Document

### 1.1.Objective

Access a confidential document.

### 1.2.Solution

The challenge requires a **confidential document** to solve it. After a little bit of reconnaissance, `/ftp` path was found in the `robots.txt` file. The `/ftp` path leads to a bunch of files, one of them being **`acquisitions.md`**, which is our required confidential file.

![Files in /ftp](img/files-in-ftp-path.png)

![Confidential Document Lab Solved](img/confidential-document-solved.png)
