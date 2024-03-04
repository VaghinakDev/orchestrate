Store Annotation AWS S3 by Role ARN

Python Version Compatibility: 3.8, 3.9, 3.10, 3.11

Dependencies:
- superannotate library, version 4.4.19 or higher
- boto3 library, version 1.28.0 or higher

This script establishes a connection to AWS based on provided credentials and stores the annotation JSON file in a specified location.

Before Running the Script:
Ensure the following environment variables are set:
- SA_TOKEN: The SuperAnnotate SDK token. This key enables automatic client initialization.
- EXTERNAL_ID: (To be defined)
- ROLE_ARN: Role ARN
- BUCKET_NAME: S3 bucket name
- AWS_ACCESS_KEY_ID: The access key for your AWS account, facilitating automatic client initialization.
- AWS_SECRET_ACCESS_KEY: The secret key for your AWS account, enabling automatic client initialization.

Instructions for Creating Secrets and Mounting to the Action in the Pipeline Canvas Page:
- Create secrets for the required environment variables mentioned above.
- Mount these secrets as environment variables in the pipeline canvas page.

The handler function triggers the script upon an event [Item annotation status updated].
