### How to connect to Amazon Web Services and download the data using command lines
###
#### Install aws client 
`sudo apt get install awscli` or `pip install awscli`
####
#### Configure aws client
`aws configure`
#### You will need AWS access keys for configuration: `aws_access_key_id` and `aws_secret_access_key`.
#### You can ignore `default AWS region` and `default output format`.
####
#### List accessible directories in AWS S3
`aws s3 ls`
####
#### Download a sub-directory to your local directory
`aws s3 sync s3://directory/subdir ~/local/subdir`
####
#### Download a sra fastq file to local 
`aws s3 cp s3://sra-pub-src-6/SRR11422700/test.fastq.gz.1 test.fastq.gz`
