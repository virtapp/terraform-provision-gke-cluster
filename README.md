Documentation

    # terraform-provision-gke-cluster 

Prerequisites

    Install terraform-provision-eks-cluster 
    Get files from source
    Example : Clone repository
    
    export GOOGLE_CREDENTIALS="/tmp/terraform-provision-gke-cluster/credentials.json"
    terraform init -upgrade
    terraform plan
    terraform apply -auto-approve
    
    kubectl config get-contexts && 
    gcloud container clusters get-credentials $(terraform output -raw kubernetes_cluster_name) --region $(terraform output -raw region)
    terraform destroy -auto-approve
