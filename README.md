# Integration_info
Use windows set for Integration task
Before starting the taks check latest Application arxml attached or not, then port excel sheet, and conan pakcages info. if anything is missing in that then ticket move to to do to defect and info to customer.
If all are seems good then click on arxmal and with raw option save to your local pc and file format cheage to all file to arxml extension. then save port excel sheet as well.
Task assigned in jira for integration. As per your zonal check your task and clone NB(Nightly build) full project folder tak into your local pc
then go to github and as per zonal create child branch from main. give name as per task.
Then in code option copy http link from github.
come to local pc where you want to keep there create one new folder and inside choose option open gitbash here.
Then give command git clone http link.
Then give command git checkout to jump branch from main to your child branch.
once done go to NB folder and copy RH850 vector package and config folder.
before that both folder pasting into your work space keep original config folder backup to the same workspace.
then paste both folders.
once done with those steps, go to option .dpa and right click on it and try to open davanci configurator.
Try to validate and generate the all modules. all modules should be 0 errors.
Once done go to Davanci developer Import option you local Application arxmal with raw data where ever you have saved that file import here.
In configurator it will ask for sync up click on okay.
Then open old and latest config folder into beyond compare to compare before integrated file and after one.
Accept UUID nothing should not be change e.g Data type. if any data type is miss mathc then there will be chance of data loss during communication.
Next go to Davanci Developer open the port connaction check each and every port has been connected as per excel sheet if any connection is looks missing make a connection as per sheet and save the all connections.
Go to file coan.py and coanan.lock file update module name with vesrion supported to both files one done save it.
once done to add your changes into git use command 

git status --> will show your changes into files
git add . --> To add all in single shot
git add file1, file2, filen etc.....
git status --> To check chaned files.
git commit -m " add your comment " --> with ira id and comment commit your changes.
git push --> To reflect your changes use the command
Then go to your barnch and once relfected your changes create PR.
Once PR created build should be done without any error.

CI 
CD


************************ Integration Testing for basic level communication ************************************************

Once all PR and junkin build passed,
