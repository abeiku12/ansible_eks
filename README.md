This playbook assumes that you have the necessary permissions, AWS CLI configured, and the Ansible boto3 and botocore dependencies installed.


Prerequisites
Install required Ansible collections:
ansible-galaxy collection install community.aws community.kubernetes
Ensure AWS CLI and eksctl are installed:
pip install awscli eksctl
Configure AWS credentials:
aws configure
Install Python dependencies:
pip install boto3 botocore

Run the Playbook
ansible-playbook aws_infra.yml

This playbook will:
1. Create an EKS cluster using eksctl.
2. Deploy Prometheus in the Kubernetes cluster.
3. Expose Prometheus via a LoadBalancer.
