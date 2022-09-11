1 - Amazon EC2 Instance:

    An Amazon EC2 instance is a virtual server in the cloud.
    Its configuration at launch is a copy of the Amazon Machine Image (AMI) that you specified when you launched the instance.
    
2 - Amazon Machine Image (AMI)

    An Amazon Machine Image (AMI) provides the information required to launch an instance.
    You must specify an AMI when you launch an instance.
    You can launch multiple instances from a single AMI when you need multiple instances with the same configuration.
    You can use different AMIs to launch instances when you need instances with different configurations.
    
3 - Launching an Instance:

    When you launch an instance, the instance type that you specify determines the hardware of the host computer used for your instance.
    Each instance type offers different compute, memory, and storage capabilities and are grouped in instance families based on these capabilities.
    
4 - Amazon EC2 Publick Key:
   
    Amazon EC2 uses public key cryptography to encrypt and decrypt login information.
    Public key cryptography uses a public key to encrypt a piece of data, and then the recipient uses their private key to decrypt the data.
    The public and private keys are known as key pair.
    
5 - Amazon EC2 Regions, Availability Zones and Local Zones.

    Amazon EC2 is hosted in multiple locations world-wide.
    These locations are composed of Regions, Availability Zones, and Local Zones.
    Each Region is a seprate geographic area that has multiple, isolated locations known as Availability Zones.
    A virtual private cloud (VPC) is a virtual network dedicated to your AWS account.
    While a VPC resides in an AWS Region a subnet must reside within a single Availability Zone.
    
6 - Amazon Security Groups:

    A security group acts as a virtual firewall that controls the traffic for one or more instances.
    When you launch an instance, you can specify one or more security groups; otherwise, the default security group is used.
    You can add rules to each security group that allows traffic to or from its associated instances.
    
6 -  Launching an Instance:
  
     When you launch an instance, the root device volume contains the image used to boot the instance.
     When you launch an instance in Amazon EC2, you have the option of passing user data to the instance that can be used
     to perform common automated configuration tasks and even run scripts after the instance starts.
     Its always a good idea to review the instance launch details you have configured before the deployment.
     An instance enters the pending state when it launches for the first time and changes to a running state when it is ready for use.
    
    
    
    
    
    
    
    
    
    
    
