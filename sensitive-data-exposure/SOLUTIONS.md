# SOLUTIONS

## 1.Confidential Document

### 1.1.Objective

Access a confidential document.

### 1.2.Solution

The challenge requires a **confidential document** to solve it. After a little bit of reconnaissance, `/ftp` path was found in the `robots.txt` file. The `/ftp` path leads to a bunch of files, one of them being **`acquisitions.md`**, which is our required confidential file.

![Files in /ftp](img/files-in-ftp-path.png)

![Confidential Document Lab Solved](img/confidential-document-solved.png)

## 2.Exposed Metrics

### 2.1.Objective

Find the endpoint that serves usage data to be scraped by a popular monitoring system.

### 2.2.Solution

The lab indicates that the **Prometheus metric system** is being used. The Prometheus metric generally serves metrics data in `/metrics`. Visit the URL to solve the challenge.

![Exposed Metrics Solved](img/exposed-metrics-solved.png)

## 3.Exposed credentials

### 3.1.Objective

A developer was careless with hardcoding unused, but still valid credentials for a testing account on the client-side.

### 3.2.Solution

After inspecting all the JavaScript files from the source, a **username** and **password** were found hardcoded in the `main.js` file on lines `11366` and `11367`.

![Username and Password](img/username-and-password.png)

![Exposed Credentials Solved](img/exposed-credentials-solved.png)
