# EC2Instance 
## Sets up remote access to a virtual server through Amazon's EC2
### STEPS:

1. Set up the Key Pair
	- proves for identity when connecting to instance

2. Create security group
	- create inbound rules: ssh access for any IP, HTTP users from any location access to web server(including myself)
	- create outbound rule: all traffic: any traffic is allowed out of EC2 instance(default)
	

3. Deploy the Instance
	- Amazon Linux AMI
	- t2.micro instance type
	- chose key pair created earlier
	- chose security group created earlier
	- configured storage: choose “8” GiB, “gp2” root volume
	- pasted a script into "user data" field under advanced details
	- NOW we are all set to launch instance

4. View Deployed Instance

5. Access the Instance
	- SSH into the server in terminal ssh -i for remote server using private key

https://medium.com/aws-tip/from-zero-to-sshero-a-step-by-step-guide-to-connect-remote-access-your-ec2-instance-using-ssh-90e713d0ce70
