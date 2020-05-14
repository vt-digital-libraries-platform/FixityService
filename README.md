# FixityService

![Overview](images/overview.png "Overview")
![Fixity workflow](images/steps.png "Fixity workflow")

# Overview
* On ingest, system upload file to S3 bucket for preservation, verify the object's integrity during the upload. 
* Everyday Fixity service checks file's last fixity check date on or before 90 days and perform fixity check on these files
* Fixity service sends daily email with a summary report (e.g. Today, fixity check # files, # matched, # mismatched, etc)

# Program Workflow
* Genereate tasks for the file's last fixity check date on or before 90 days
* Execute fixity check pipeline
* Send daily email with a summary report (e.g. Today, fixity check # files, # matched, # mismatched, etc) 

# Doc
* https://webapps.es.vt.edu/confluence/display/LIBTD/DLP%3A+Fixity+Service
* https://webapps.es.vt.edu/confluence/display/LIBTD/Digital+Libraries+Platform
* https://aws.amazon.com/premiumsupport/knowledge-center/data-integrity-s3/

