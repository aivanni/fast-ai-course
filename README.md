# Practical Deep Learning for Coders (fast.ai courses)

## Setup

* Updated the ami to use 30gb ebs volume instead of default 128gb.
* Just run `./setup/setup_t2.sh` to get t2 and if we need gpu then run `./setup/setup_p2.sh`.
* Use `us-west-2` as the region for aws as the ami is for that region. 

## Some Useful Commands

* to get list of everything running. 

```
for region in `aws ec2 describe-regions --output text | cut -f3`
do
     echo -e "\nListing Instances in region:'$region'..."
     aws ec2 describe-instances --region $region
done
```

* dl_course is the password for the default notebook. 
* Use the remove file to remove the instance. It will terminate the instance and take care of ip address and ebs volume. 
* To start over, delete key from local machine and delete pair from aws. 


