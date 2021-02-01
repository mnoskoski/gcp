---
GCP-CLI:
    title: 'Commands GCP CLI'
---

## GOOGLE CLOUD - Commands CLI


+ Command Login: 
    gcloud auth login

+ Command set Project: 
    gcloud config set project PROJECT_ID

+ Pegando o ID do project:
    gcloud config get-value project

+ Pegando o numero do projeto:
    PROJECT=(gcloud config get-value project)
    echo topazio && gcloud projects list --filter="topazio" --format="value(PROJECT_NUMBER)"



gcloud projects add-iam-policy-binding topazio \
--member=serviceAccount:service-576396400081@containerregistry.iam.gserviceaccount.com --role=roles/containerregistry.ServiceAgent