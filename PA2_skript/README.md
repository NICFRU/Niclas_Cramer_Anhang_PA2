# Usage:
before execution of the script execute following lines if not already satisfied  
- python get-pip.py
- pip install pip
- pip install -r requirements.txt

# Execution of the script 
- copy raw data into the "RawData" folder
- change variables in Config.py
- execute Config.py
    - the folder structure will be created
    - the files will be automaticly created 
- execute Multi_app 
    -  go to path:  http://127.0.0.1:8082



## Elements before execution 
-	Apps
    -	app_overview.py
-	modules
    -	converter.py
    -	create_app_for_files.py
    -	create_colective_app_script.py
    -	create_SQL_file.py
    -	overall_funktions.py      
-	RawData --> saving the raw data files into this folder
-	Config.py  execute all modules 
-	README.md
-	Requirements.txt
- navigate to the config.py file or open it in a notepad or VSC/ Pycharm and edit the variables
- execute the script in VSC/ Pycharm 
or navigate with the cmd to the folder where the config.py file with: python3 config.py or config.py



## Folder structure after execution

- Apps
- Logging_files
- Modules
    - converter.py
    - create_app_for_files.py
    - create_colective_app_script.py
    - create_SQL_file.py
    - overall_funktions.py
- Picture
    - Html aller erstellten Grafiken
- Processed
- RawData
- Sql_files
- Config.py
- Multi_app.py
- README.md
- Requirements.txt

# overview

## Config.py 
-	Combines the execution of the other tables together to have a single entity for the execution of the whole process


## Multi_app.py 
-	The initial program to start the visual inside of the tables 


## converter.py 
-	 Pre-processes the csv or txt file with converter.py script
-	Identifies lines with too many column separators 
-	Deletes those extra semicolons and saved file to processed - MANUALLY! based on file.txt in the Logging_files folder:
-	replaces quotation marks and values which represent an empty value 
-	creates an overview of the data in the logging folder

## create_SQL_file.py
-	Creates SQL import script with create_SQL_file.py
-	Generated script can be used to import to SQL db (DB must  be created first)


## create_colective_app_script.py 
-	Creates a script, which is a collected  script of the visual representation of the files


## create_app_for_files.py
-	Generates scripts which allows a overview of the table to get an inside of the meta information 


## overall_funktions.py
-	Contains functions for the other modules to use

