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
    aws eks --region us-east-2 update-kubeconfig --name "education-eks-GcR1ym71"
    terraform destroy -auto-approve
