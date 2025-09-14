# dev-quick-start
A cheatsheet of commands that I always forget

Creating Python virtual environment
- `python3 -m venv .venv`
- `source .venv/bin/activate`
- `pip3 install google-adk==1.8.0 # packages`

GCP authentication
- `gcloud auth login`
- `gcloud auth application-default login`

GCP add IAM policy binding
- `gcloud projects add-iam-policy-binding <PROJECT_ID> --member="<SERVICE ACCOUNT>" --role="roles/<ROLE>" --project=<PROJECT_ID>`
