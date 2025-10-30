echo "Launching EC2 Instance..."

aws ec2 run-instances   --image-id ami-0c02fb55956c7d316   --instance-type t2.micro   --key-name mykey   --security-group-ids sg-1234567890abcdef   --subnet-id subnet-123456   --tag-specifications 'ResourceType=instance,Tags=[{Key=Name,Value=DevOps-Server}]'

echo "EC2 Instance launch command executed!"
