## Create a new s3 bucket

```md
aws s3 mb s3://checksums-examples-xy-1235
```

## Create a file that we will do a checksum on 

```
echo "Hello Sope" > myfile.txt
```
## Get a checksum of a file for md5
md5sum README.md

#89b4aa6c5571848c4ae5688793d79046  README.md

## Upload a file 
```
aws s3 cp myfile.txt s3://checksums-examples-xy-1235
```