==============================================================================================================================

Website Setup Guide

1. Download raw data
    https://onedrive.live.com/?id=B432689A86B2CE06%21sb0033c43999b4a2eb6078f156d0aeefb&cid=B432689A86B2CE06&redeem=aHR0cHM6Ly8xZHJ2Lm1zL2YvYy9iNDMyNjg5YTg2YjJjZTA2L0VrTThBN0NibVM1S3RnZVBGVzBLN3ZzQkhHMUNHYklSejdkaGlTSjJDUVEzWlE%5FZT01OjZSOUtQMSZzaGFyaW5ndjI9dHJ1ZSZmcm9tU2hhcmU9dHJ1ZSZhdD05

2. Download and active all required application (Apache, MySQL, XAMPP)
3. In MySQL command client, run the following command. It return the path to the principal directory to store the input files.

    SELECT @@secure_file_priv;

4. Copy all sample data and real data files to the above address. If you are not using MySQL 8.0 or did not download MySQL by default, replace the path in read-sample.sql by your path.

5. In MySQL command client, run read-sample.sql by following command to set up sample database:

    source [path to read-sample.sql];

6.  In MySQL command client, run read-production.sql by following command to set up sample database:

    source [path to read-production.sql];

7. If you set the mysql password, type it in config.php

8. In any browser, search localhost/index.php to open the web. (If you are using xampp, you need to copy all files in directory WebsiteSetup to xampp/htdocs)

==============================================================================================================================

Features:


1. Basic search feature (search by exact title and print details).
2. User login/register.
3. Top navigate bar.
4. User history (NEW)
5. User comment (NEW)
6. User rating (NEW)
7. Movie detailed information (NEW)
8. The 5 most popular movies in main page (NEW)

==============================================================================================================================

File Description:


1. Directory DatabaseSetup store sql files to setup the databases (C2,C3,C4)
2. Directory SampleDatbase store csv file containing sample data.
3. Directory WebsiteSetup store php files to setup the web (C5)
4. README.md (C1)