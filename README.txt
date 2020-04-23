Udacity Cloud DevOps Engineer

Project 2 - Deploy a high-availability web app using CloudFormation
To create stack : 
./create.sh project2iaac projectinfra.yml network-parameters.json
OR
aws cloudformation create-stack --stack-name project2iaac --capabilities CAPABILITY_IAM --template-body
file://projectinfra.yml --parameters file://network-parameters.json --region=us-west-2

Update Stack:
./update.sh project2iaac projectinfra.yml network-parameters.json
OR
aws cloudformation update-stack --stack-name project2iaac --capabilities CAPABILITY_IAM --template-body
file://projectinfra.yml --parameters file://network-parameters.json --region=us-west-2

Delete Stack:
aws cloudformation delete-stack --stack-name project2iaac

