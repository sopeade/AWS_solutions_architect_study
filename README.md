
# Relevant links
https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell-on-windows?view=powershell-7.5#winget
https://docs.aws.amazon.com/powershell/latest/userguide/pstools-getting-set-up-windows.html
https://docs.aws.amazon.com/powershell/latest/reference/   #a powershell guide
https://docs.aws.amazon.com/cli/latest/   # a bash/cli guide
https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html  #installing the aws cli
https://stackoverflow.com/questions/56314710/the-term-conda-is-not-recognized-as-the-name-of-a-cmdlet
https://docs.aws.amazon.com/cli/latest/reference/cloudformation/
Install powershell 7 +
winget install --id Microsoft.PowerGetGet-HShell --source winget

Get-Host  # Check and confirm powershell 7 + Need to ensure powershell 
sudo apt-get install -y powershell
Install-Module -Name AWS.Tools.Installer
Install-AWSToolsModule AWS.Tools.S3 -CleanUp   # Can execute powershell commands

Commands
aws s3api list-objects --bucket my-example

New-S3Bucket #Create s3 bucket
e.g. New-S3Bucket -BucketName my-powershell-bucket-123

Setup:
Step 1:
Install AWS ClI

41:55
#Install or update the AWS CLI

msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi   # windows
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install     #linux

aws sts get-caller-identity
# Unable to locate credentials. You can configure credentials by running "aws configure".
IAM-> users-> create user -> on selecting created user -> security credentials -> Create access key
command line interface#AWS_Solutions_architect_study


iac - Infrastructure as code