# CD12352 - Infrastructure as Code Project Solution
# [CRISTINE LANTING]

## Spin up instructions
Run ./sh-files/install.sh stack-project2 network.yml network-parameters.json
Run ./sh-files/install.sh udagram-stack-project2 udagram.yml udagram-parameters.json
## Tear down instructions
Run ./sh-files/delete.sh stack-project2 network.yml network-parameters.json
Run ./sh-files/delete.sh udagram-stack-project2 udagram.yml udagram-parameters.json

## Other considerations
The following should be installed in VSCode
- AWS Toolkit
- Git bash for windows, instructions can be found here > https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal

Other note: user should be on the folder above ssh-files before running the script. On this case it should be on -cd12352-Deploy-Infrastructure-as-Code-project-clanting

## Updated the following based on review
Review 1: Add a output section showing the Load Balancer DNS URL
- Solution: updates are available from line 162 under 'udagram.yml'

Review 2: Please change the instance type to meet the minimum requirement
- Solution: Update available on line 60 under 'udagram.yml'. Changed to t3.small

Review 3: Provide a URL to your deployed app. In this way, I can verify your deployment.
- Link can be accessed in: http://udagra-WebAp-naRDxzwW1CRu-218369682.us-east-1.elb.amazonaws.com