# Virtual Private Cloud

## What is a Virtual Private Cloud?
A virtual private cloud (VPC) is a private cloud computing environment hosted within a public cloud. A virtual private cloud reserves its some of its resources to be accessed by a single customer in a pool of a crowded public cloud with various customers assessing computing resources. 

![virtual-private-cloud](https://github.com/yiwei-chay/networking-notes/assets/146081571/f985e0df-df1f-493a-920b-7e722fae6165)

## Public Cloud vs Private Cloud vs Virtual Private Cloud (VPC)
In a public cloud, resources such as servers and storage are owned and operated by a third-party cloud service provider and delivered over the internet. The cloud service provider has the sole responsibility for all management and maintenance of the system. Public cloud deployments are **faster than on-premises infrastructures** and with an **almost infinitely scalable platform**. These deployments are generally used to provide web-based email and testing and development environments. Some of the advantages of public clouds include:
- Lower costs
- High reliability
- Scalability
- No maintenance

A private cloud, on the other hand, are services offered either over the Internet or a private internal network. Only selected users instead of the general public are allowed to use this service. Private clouds gives businesses the benefits of hosting in a public cloud - such as scalability and elasticity. It also provide additional benefits including **higher level of security and privacy** through both company firewalls and internal hosting, ensuring that sensitive data will not be accessible to third-party providers. However, one major drawback is that it **requires the same management and maintenance expenses** as traditional datacenter ownership as companies are accountable to managing the private cloud. 

A virtual private cloud (VPC) is a private cloud within a public cloud; no one else shares the VPC with the VPC customer. It is a unique combination of a public and private cloud. It offers services by generating an isolated section within a public cloud. This segmented region of the public cloud functions as a lone private cloud model and renders services observed in private cloud deployments. Through VPC, companies have benefits of enhanced privacy over their private cloud models and save on costs related to public cloud deployment. However, some weaknesses of VPC includes:
- Restrictive customisation
- Outage problems: VPC architecture is prone to outages and failures, **due to customers' customisations on the VPC**

## How does VPC work?
VPC runs on shared infrastructure like a public cloud. It offers a level of isolation between cloud customers sharing resources, achieved through several methods:
1. IP Subnets  
IP subnets are a range of addresses reserved for VPC users, dividing part of the network for private use. They are not accessible via the public internet and are not publicly visible. Subnets partitions the networks through the third layer of the OSI model (further explored in the section below).

2. VLAN  
LAN (local area network) is a group of computing devices that are connected together without the need of the internet. It is a way of separating the VPC from the public cloud via the second layer of the OSI model.

3. VPN (virtual private network)  
VPN traffic passes through publicly shared internet infrastructure but uses encryption to create a private network above the public network, and is not visible to anyone.

### OSI model
The OSI model is a universal structure for computer networking. It splits the communication system into 7 abstract layers, each handling a specific job and communicates with the layers above and below itself. The layers give engineers a better idea of how the transmittion of data works as well as the ability to narrow down problems whilst debugging. 

<img width="1003" alt="OSI-model" src="https://github.com/yiwei-chay/networking-notes/assets/146081571/f8fdbdee-97a5-48e9-a0a0-1c7054b6ca59">


