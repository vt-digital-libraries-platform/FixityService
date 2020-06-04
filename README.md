# FixityService

![Overview](images/overview.png "Overview")
![Fixity workflow](images/steps.png "Fixity workflow")

# Overview
* On ingest, system upload file to S3 bucket for preservation, verify the object's integrity during the upload. See [Check the integrity of an object uploaded to Amazon S3](https://aws.amazon.com/premiumsupport/knowledge-center/data-integrity-s3/).
    * Fixity Service performs the initial fixity check on each uploaded file.
* Everyday Fixity service checks file's last fixity check date on or before 90 days and performs fixity check on these files
* Fixity service sends a daily email with a summary report only when there is a "MISMATCHED" event occurred. (e.g. Today, fixity check, there are # mismatched, the location of files, filename, etc).

# Launch CloudFormation stack
[![Launch Stack](https://cdn.rawgit.com/buildkite/cloudformation-launch-stack-button-svg/master/launch-stack.svg)](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/new?&templateURL=https://steps-fixity-us-east-1.s3.amazonaws.com/steps-fixity-solution/version1/serverless-fixity-for-digital-preservation-compliance.template)

# DLP doc
* https://webapps.es.vt.edu/confluence/display/LIBTD/DLP%3A+Fixity+Service
* https://webapps.es.vt.edu/confluence/display/LIBTD/Digital+Libraries+Platform

# Special thanks to
* [Serverless Fixity for Digital Preservation Compliance](https://aws.amazon.com/solutions/implementations/serverless-fixity-for-digital-preservation-compliance/)
