 ## Create a bucket
aws s3 mb s3://sopes-random-bucket-z1

 ### Create a new file
echo "my new file" > hello.txt

## Upload file with metadata
aws s3api put-object --bucket sopes-random-bucket-z1 --key hello1.txt --metadata color=beige

## Get Metadata through head object
aws s3api head-object --bucket sopes-random-bucket-z1 --key hello1.txt
