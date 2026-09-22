# oracle_pdb_ass_II_20251IMA043_kundwa
AUCA PL/SQL assignment II - Oracle PDB 
**# Assignment 2 - Oracle PDB Management

**Name:** Kundwa Nkwaya Kelche  
**Student ID:** 20251IMA043  
**Course:** Database Development with PL/SQL**
## Overview
This repository contains my submission for Individual Assignment II. In this assignment, I created and managed Oracle 19c Pluggable Databases (PDBs) using SQL*Plus and checked the status using Oracle Enterprise Manager (OEM)

### Task 1: Creating Permanent PDB and User
1. Opened SQL*Plus as `SYSDBA`.
2. Created my permanent database `ku_pdb_20251IMA043`
3. Opened the database with `ALTER PLUGGABLE DATABASE ku_pdb_20251IMA043 OPEN;`.
4. Switched to my new database container and created user `kundwa_plsqlauca_20251IMA043`

5. ## Task 2: Creating and Deleting Temporary PDB
1. Switched back to the root container (`CDB$ROOT`).
2. Created a temporary database named `ku_to_delete_pdb_20251IMA043`.
3. Checked that it was created using `SHOW PDBS;
4. Deleted the database and its files using `DROP PLUGGABLE DATABASE ku_to_delete_pdb_20251IMA043 INCLUDING DATAFILES;
5.  Ran `SHOW PDBS;` again to confirm it was removed

6.  ### Task 3: Enterprise Manager Screenshot
1. Logged into Oracle Enterprise Manager in my browser at **`https://localhost:5500/em`**
2. Took a screenshot of the main database dashboard page showing the database

##Challenges
** When trying to close the temporary database, it said it was already closed because new PDBs start in `MOUNTED` status[cite: 7]. I was able to drop it
