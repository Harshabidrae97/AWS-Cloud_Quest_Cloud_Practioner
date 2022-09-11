1 - Amazon EC2:

    Amazon EC2 offers the broadest and deepest compute platform with choice of processor,
    storage, networking, operating system, and purchase model.
    
    Amazon EC2 instances provide virtual compute capacity in the cloud.
    
    Information about the instance such as its public IP, private IP, and public DNS is displayed in the Instance
    summary panel by selecting the Amazon EC2 Instance.
    
    Amazon EC2 provides a wide selection of instance types that belong to instance families
    that are optimized to fit different use cases.
    
    Each instance type includes one or more instance sizes, allowing you to scale your
    resources to the requirements of your target workload.
    
    The Amazon EC2 console allows you to filter instance attributes such as
    instance type, instance family and instance size. You can search using
    keywords, attribute name or expressions.
    
    Instance metadata is data about your instance that you can use to configure
    or manage the running instance. Instance metadata is divided into categories,
    for example, host name, events, and security groups.
    
    When creating a new instance, you can enable the Instance Metadata Service
    (IMDS) using the Advanced Details section. This will allow you to display
    attribute details using the instance's public IP.
    
    You have the flexibility to connect to an Amazon EC2 instance using EC2 Instance Connect, Session
    Manager, or an SSH Client
    
    Amazon EC2 Instance Connect provides a simple and secure way to connect to 
    your Linux instances. EC2 Instance Connect uses (IAM) policies and principles
    to control SSH access to your instances, removing the need to share and manage
    SSH keys
    
    
    Session Manager lets you manage yout Amazon EC2 instances through an interactive
    one-click browser-based shell or through the AWS CLI. Once the seesion begins, you
    can run bash commands as you would through any other connection type.
    
    You can connect to your instance using an SSH client on your local computer using your instance key 
    pair. Your computer may have an SSH client by default or you may need install an SSH client.
    
    
    The EC2 Instance Connect API pushes a one-time-use SSH public key to the instance metadata
    for 60 seconds. An IAM policy authorizes your IAM user to push the public key to the instance metadata.
    The SSH daemon on the instance uses the AuthorizedKeysCommand and AuthorizedKeysCommandUser 
    to access the public key from the metadata to authenticate and connect you to the instance.
    
     Once you are connected to the instance you can control the instance using CLI commands.
     The command prompt behaves as if you were connected locally.
     
     The Actions menu allows you to control the instance state and modify instance attributes.
     
     You can also use instance metadata to access user data that you specified when launching
     your instance.
     
     The Instance state menu allows you to place an instance into different states
     of activity. You can start and stop an instance if it has an Amazon EBS volume
     as its root device.
     
     Once the instance is stopped, CPU usage and data transfer charges cease, but
     storage charges for any attached Amazon EBS volumes continue.
     
     Each time you start a stopped instance, AWS charges a minimum of one minute
     for usage per-second billing instances. After one minute, AWS charges only for the seconds
     you use.
     
     You must stop your Amazon EBS-backed instance before you can change its instance type.
     Ensure that you plan for downtime while your instance is stopped. Stopping the instance
     and changing its instances type might take a few minutes, and restarting your instance 
     might take a variable amount of time depending on your applicaiton's startup scripts.
    
    
    
    
    
