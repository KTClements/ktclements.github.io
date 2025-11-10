[Back to Portfolio](./)

ClinVar Data Query Portal
===============

-   **Class: CSCI 495 - Systems Analysis and Software Design** 
-   **Grade: A** 
-   **Language(s): JavaScript (Node.js), HTML/CSS, SQL** 
-   **Source Code Repository:** [features/mastering-markdown](https://guides.github.com/features/mastering-markdown/)  
    (Please [email me](mailto:example@csustudent.net?subject=GitHub%20Access) to request access.)

## Project description

A web-based query portal for ClinVar genetic variant data built with Node.js and MySQL. The application automatically downloads and processes variant data from ClinVar's FTP site weekly, allowing researchers and healthcare professionals to search, filter, and export specific subsets of genetic variant information. Features include automated database synchronization, multi-column filtering, keyword search, and export functionality in CSV and tab-delimited formats compatible with Microsoft Access. Designed to simplify access to ClinVar's extensive genetic variant database for clinical researchers, genetic counselors, and bioinformatics professionals who need targeted data without managing bulk downloads.

## How to compile and run the program

1. Install Node.js and MySQL server with workbench
2. Clone the repository
3. Install dependencies:
```bash
npm install
```
4. Configure MySQL connection in `index.js` with your local credentials
5. Create the database by running `databaseCreation.sql` in MySQL Workbench
6. Start the server:
```bash
node index.js
```
7. Access the application at `localhost:3000` or your system's IPv4 address on the local network

## UI Design

Access the web interface to view the last database update date and begin querying. Select columns from the dropdown menu and enter keywords in the search bar to filter genetic variant data. The interface displays your search history and shows when a query is processing. Once complete, download the filtered results in CSV or tab-delimited format for import into Microsoft Access or other analysis tools.

![screenshot](images/dummy_thumbnail.jpg)  
Fig 1. The launch screen

![screenshot](images/dummy_thumbnail.jpg)  
Fig 2. Example output after input is processed.

![screenshot](images/dummy_thumbnail.jpg)  
Fig 3. Feedback when an error occurs.

## 3. Additional Considerations

Requires Node.js 14+ and MySQL 8.0+. Tested on Windows 10 and deployed on GoDaddy shared hosting with Nginx.

For more details see [GitHub Flavored Markdown](https://github.com/Racabane/CSCI_495_RED_TEAM/blob/4c2ecd9059c9faedd5e883c79e980f3b8c5423b8/README.md).

[Back to Portfolio](./)
