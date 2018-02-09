# vsp
vsp thoi


ssh -i "123.pem" ubuntu@ec2-52-205-11-198.compute-1.amazonaws.com



I would like to connect with
A standalone SSH client
A Java SSH Client directly from my browser (Java required)
To access your instance:
Open an SSH client. (find out how to connect using PuTTY)
Locate your private key file (123.pem). The wizard automatically detects the key you used to launch the instance.
Your key must not be publicly viewable for SSH to work. Use this command if needed:
chmod 400 123.pem
Connect to your instance using its Public DNS:
ec2-52-205-11-198.compute-1.amazonaws.com
Example:
ssh -i "123.pem" ubuntu@ec2-52-205-11-198.compute-1.amazonaws.com
Please note that in most cases the username above will be correct, however please ensure that you read your AMI usage instructions to ensure that the AMI owner has not changed the default AMI username.
If you need any assistance connecting to your instance, please see our connection documentation.
