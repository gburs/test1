Installation Steps:
1. Create folder: "C:\TESTS\Toogood" and unzip the Test1.zip file in this folder;
2. Run in MSSQL2008R2 under sysadmin role account the script from file: "Script To Run in MSSQL2008R2.sql";
3. Desktop application in folder "Transform" is written in VS2010;
4. RunApplication folder has the minimum configuration and executable;
5. Change configuration file: "Transform.exe.config" and within the setting name "CDB" change value to match your server name;
6. Transformation sample files are in folder: "SampleTransformFiles".



Notes:
1. A user will be created in SQL with sysadmin role, however, owner privileges on database "ToogoodMaster2" are sufficient;
2. Extension to other import formats is controlled from the definition tables which start with "def_" and has field names self-explanatory;
3. The screen controlling the definition tables was not done. For new import formats follow the model in Format 1 and Format 2 in all the def_ tables and input them manually in the natural order of the foreign keys, which are activated;
4. The application screen is self-explanatory, however, if the Input Format dropdown is not populated at runtime, you have a database connection issue, check with your admin;
5. Within the application press the button "Generate Output File" and the missing prerequisites will be made available to you;
6. The case of a comma inside the field is not supported. See test file: "Sample 3 -  File Format 1";
7. Rejected record file is the full name of the input file with added ".err" extension. It gives information of all errors found including multiple errors per record;
8. Output target file is the full name of the input file with added ".out" extension.

