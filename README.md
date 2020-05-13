# FixityService

![Overview](images/overview.png "Overview")
![Fixity workflow](images/steps.png "Fixity workflow")


# Workflow
* On ingest, a checksum should be created and stored in the metadata store.
* Do fixity check daily for the files uploaded to S3 every 90 days
* Send daily email with a summary report (e.g. Today, fixity check # files, # matched, # mismatched, etc) 

# Doc
* https://webapps.es.vt.edu/confluence/display/LIBTD/DLP%3A+Fixity+Service
* https://webapps.es.vt.edu/confluence/display/LIBTD/Digital+Libraries+Platform


