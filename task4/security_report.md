# Security Implementation Report – CodTech Task 4

## Objective
To implement secure cloud storage using IAM policies, encryption, and restricted access.

## AWS Implementation
- Created S3 bucket `codtech-task4-bucket`.
- Enabled default SSE-S3 encryption.
- Applied least-privilege IAM policy (`iam_policy_aws.json`).
- Added bucket policy to enforce TLS and deny public access (`bucket_policy_aws.json`).
- Enabled S3 access logging and AWS CloudTrail for monitoring.

## GCP Implementation
- Created Cloud Storage bucket `codtech-task4-bucket`.
- Enabled CMEK encryption key for data security.
- Created a service account with only object admin access.
- Applied IAM bindings to restrict access to authorized identities.

## Conclusion
The simulated setup demonstrates how to secure cloud storage on both AWS and GCP with encryption, least-privilege IAM, and monitoring.
