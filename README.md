### Project Title - Deploy a high-availability web app using CloudFormation
### How to run the Deploy the Infrastructure?
You can run the infrastructure scripts in two easy steps:
```bash
# Ensure that the AWS CLI is configured before runniing the command below
# Create the network infrastructure
# Check the region in the create.sh file
./create.sh Network Network.yml NetworkParams.json
# Create servers
# Change the AMI ID and key-pair name in the servers.yml
# Check the region in the create.sh file
./create.sh Servers Servers.yml ServersParams.json
# Create the jump box
./create.sh JumpBox Jumpbox.yml JumpboxParams.json

```
### Infrastructure Diagram
See JPEG file for the infrastructure diagram