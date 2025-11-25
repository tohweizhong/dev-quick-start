# dev-quick-start
A cheatsheet of commands that I always forget

Creating Python virtual environment
- `python3 -m venv .venv`
- `source .venv/bin/activate`
- `pip3 install google-adk==1.8.0 # packages`

GCP authentication
- Authorize: `gcloud auth login`
- ADC login: `gcloud auth application-default login`
- Set project: `gcloud config set project weizhong-project03`
- (Set quota project: `gcloud auth application-default set-quota-project weizhong-project03`)

GCP add IAM policy binding
- `gcloud projects add-iam-policy-binding <PROJECT_ID> --member="<SERVICE ACCOUNT>" --role="roles/<ROLE>" --project=<PROJECT_ID>`

Set environment variables
- `source ./set_vars.sh`
- Example `set_vars.sh`
```
export GOOGLE_CLOUD_LOCATION="us-central1" # Example location

```


Add environment variables into bash profile
- `echo 'export GOOGLE_CLOUD_PROJECT="<PROJECT_ID>"' >> ~/.bash_profile`
- `echo 'export GOOGLE_CLOUD_LOCATION="REGION_ID"' >> ~/.bash_profile`
- `echo 'export GOOGLE_GENAI_USE_VERTEXAI=true' >> ~/.bash_profile`
- `source ~/.bash_profile`

List of git commands that I always forget
- https://github.com/tohweizhong/git-quick-start