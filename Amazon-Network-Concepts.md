1 - When was Amazon EC2 first launched:
 
    AWS lanunced its very first Amazon EC2 instance in August, 2006
    
2 - Amazon VPC:

    Amazon VPC enables you to lunch AWS resources into a virtual network that you've
    defined. This virtual network closely resembles a traditional network that you'd
    operate in your own data center with the benefits of using the scalable 
    infrastructure of AWS.
    
3 - What is a Subnet:

    A subnet is a range of IP addresses in your VPC. You can launch AWS
    resources into a specified subnet. Each subnet must reside entirely 
    within one Availability Zone and cannot span zones.
    
4 - What is a Route Table:

    A route table contains a set of rules, called routes, that are used to
    determine where network traffic from your subnet or gateway is directed.
    Use a public subnet for internet connected resources and a private subnet
    for non-internet connected resources.
    
 5 - The CIDR:
 
     The CDIR naming convention 0.0.0.0/0, represents all IPv4 addresses 
     (::/0 for IPv6)
     
 6 - What is a NAT:
 
     A NAT gateway is a Network Addressing Translation (NAT) service. You can
     use a NAT gateway so that instances in a private subnet can connect to
     services outside your VPC but external services cannot initiate a connection 
     with those instances.
     
 7 - Internet Gateway:
 
     An internet gateway serves two purposes: to provide a target in your VPC route tables
     for internet-routable traffic, and to perform network address translation (NAT)
     for instances that have been assigned public IPv4 addresses.
     
     An internet gatewat supports IPv4 and IPv6 traffic. It does not cause 
     availability risks or bandwidths constraints on your network traffic.
     There is no additional charge for having an internet gateway in yout account.
     
 8 - Security Groups:
 
     For each security group, you add rules that control the traffic
     based on protocols and port numbers. There are seprate sets of rules
     for inbound traffic and outbound traffic.
     
     You can create a security group and add rules that reflect the role
     of the instance that's associated with the security group. For example,
     an instance that's configured as a web server needs security group rules
     that allow inbound HTTP and HTTPS access. Likewise, a database instance
     needs rulees that allow access for the type of database, such as access
     over port 3306 for MySQL.
     
     Security groups are stateful. For example, if you send a request 
     from an instance, the response traffic for that request is allowed
     to reach the instance regardless of the inbound security group rules.
     Responses to allowed inbound traffic are allowed to leave the instance,
     regardless of the outbound rules.
     
     
   9 - VPC:
   
       When you create a VPC, it comes with a default security group.
       You can create additional security groups for each VPC.
       
 10 - To deploy a working internet gateway the following must be completed:
 
 
      Attach the internet gateway to VPC.
      Route tables associated with your public subnet must have a route to your internet gateway.
      Security groups associated with your VPS must allow traffic to/from the internet.
      Any instances in the VPC must have a public IP or Elactic IP address assigned.
 
 
 
 
 
 
 
 
 
