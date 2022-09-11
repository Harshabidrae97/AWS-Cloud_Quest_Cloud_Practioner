1 - Amazon VPC:

    Amazon VPC is a service that lets you launch AWS resources in a logically
    isolated virtual network that you define. You have complete control over your virtual 
    networking environment.
    
    By default Amazon VPCs are isolated from each other. A VPC peering connection is
    a networking connection between two Amazon VPCs that enbales you to route traffic between
    them using private IP addresses.
    
    By default, Amazon VPCs cannot communicate with resources in other Amazon VPCs
    using private IPv4 addresses or IPv6 addresses. In this case the Financial Services 
    Server doesn't have a public IP, therefore your Amazon VPCs are unaware how to route data to
    private IP destinations outside of their own private range.
    
    Instances in either Amazon VPC can communicate with each other as if they are within
    the same network.
    
    Your Amazon VPC will request that Amazon VPC allow access to its resources.
    The Amazon VPC making the request is called the Requester. You can request access to
    Amazon VPCs from other AWS accounts.
    
    To request a VPC peering connection with an Amazon VPC in your account,
    ensure that you have the IDs of the Amazon VPCs with which you are
    creating the VPC peering connection. You must both create and accept
    the VPC peering connection request yourself to activate it. If the 
    peering connection is across accounts, both accounts must accept the
    connection to activate it.
    
    After you establish a peering connectio, you must modify the route
    table associated with each Amazon VPC. You must add a route into each route
    table to allow traffic to be routed to the peered Amazon VPC.
    
    Just because Amazon VPCs are peered doesnt mean that all the data is accepted.
    Security features such as network access control lists and security groups will still
    apply. Be sure to update them accordingly.
    
    Your services can communicate once your Amazon VPCs are peered, and
    security groups allow the correct traffic. Remember, if you need to add
    different traffic types, you will have to chnage the inbound rules of
    your security groups.
    
 2 - Connecting to an Amazon EC2:
 
     There are four ways to connect into an Amazon EC2 instance: EC2 Instance
     Connect, Session Manager, an SSH client, and EC2 Serial Console.
     
     Amazon EC2 Instance Connect provides a simple and secure way to connect to
     your Linux instances using Secure Shell (SSH). With EC2 Instance Connect,
     you use AWS Identity and Access Management policies and principles to
     control SSH access to your instances, removing the need to share and manage SSH keys.
     All connection requests using EC2 Instance COnnect are logged to AWS CloudTrail so 
     you can audit connection requests.
     
     Amazon EC2 instances reside within a subnet. A subnet of IP addresses in 
     your Amazon VPC.
     
 3 - Route Table:
 
     One important property of a subnet is its route table. A route table
     contains a set of rules called routes. Routes are used to determine where
     network traffic from your subnet or gateway is directed.
     
     Route tables will have rules for local traffic and public IP ranges if
     a gatewat is attached. Note that AWS recommends that you specify a CIDR
     block from the private IPv4 address ranges as specified in RFC 1918.
     
     Route tables have a target: The gateway, network interface, or connection
     throught which to send the destination trafic. Peering connections are one
     type of connection that can be used as a target.
     
     The route tables for each Amazon VPC must be modified to allow traffic across
     the peering connection.
     
 4 -  Secure Groups:
 
      Security groups do not automatically accept data from peered Amazon VPCs.
      You must update security groups to allow your peered Amazon VPC as an incoming
      source.
      
      Security groups are stateful-if you send a request from your instance, the response 
      traffic for that request is allowed to flow in regardless of the inbound rules. This 
      also means that responses to allowed inbound traffic are allowed to flow out, regardless 
      of the outbound rules.
      
      Security group rules are always permissive; you can't create rules that deny
      access. Security group rules enable you to filter traffic based on protocols
      and port numbers.
     
     
     
     
     
     
     
    
