﻿# Farma_Extra_Baik_SQL_Database_Project
This a complete database structure to create a POS for a pharmacy, the database model is on the Third Normal Form and its ready to deploy.

There is a backup sample that can be restore on SQL Server, to restore the database follow these instructions:


1. Open Microsoft SQL Server Management Studio, and navigate to Databases:

2. Right-click Databases, and click Restore Database.  In the Source for restore section, select From Device, and click the browse button:

3. Click Add in the Specify Backup window.  Browse to the location of your recently restored flat files. Choose the Full backup file which should be the first backup file in the list:

4. Click OK; the Specify Backup window displays:

5. Click OK. In the Destination for restore section, select the database to which you wish to restore, and in the Select the backup sets to restore section, select the backup file you selected above in step 3:

6. In the left pane, click Options, and select the following:
In the Restore options section, select Overwrite the existing database (WITH REPLACE), and leave the other options unselected.
In the Recovery state section, select Leave the database non-operational, and do not roll back uncommited transactions. Additional transaction logs can be restored. (RESTORE WITH NORECOVERY):

7. Click OK to perform the restore.
Complete these steps for each incremental backup file, including the .tm file, until you reach the incremental file containing the point-in-time file to which you wish to restore.
