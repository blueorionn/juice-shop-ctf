# Confidential Document

## Objective

Access a confidential document.

## Solution

The challenge requires a **confidential document** to solve it. After a little bit of reconnaissance, `/ftp` path was found in the `robots.txt` file. The `/ftp` path leads to a bunch of files, one of them being **`acquisitions.md`**, which is our required confidential file.

![Files in /ftp](img/files-in-ftp-path.png)

![Confidential Document Lab Solved](img/confidential-document-solved.png)
