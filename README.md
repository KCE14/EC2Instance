# EC2Instance 
Sets up an EC2 Instance using SSH
STEPS:

1. I set up the Key Pair
	- proves for identity when connecting to instance

2. Created security group
	- created inbound rules: ssh access for any IP, HTTP users from any location access to web server(including myself)
	- created outbound rule: all traffic: any traffic is allowed out of EC2 instance(default)
	

3. Deploy the Instance
	- Amazon Linux AMI
	- t2.micro instance type
	- chose my key pair i created earlier
	- chose my security group i created earlier
	- configured storage: chose “8” GiB, “gp2” root volume
	- pasted a script into "user data" field under advanced details
	- NOW we are all set to launch instance

4. View Deployed Instance

5. Access the Instance
	- SSH into the server in terminal ssh -i for remote server using private key
