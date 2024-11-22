# Portfolio-2

## Aims
A sandboxed network provides an essential learning environment and platform, offering a secure, isolated space to simulate real-world network scenarios without introducing risks to live systems. For this Portfolio, you will create your own private sandboxed virtual network using VirtualBox. The network will consist of multiple virtual machines (VMs) configured within a private IP address range. The aim is to gain an applied understanding of networking concepts, IP subnetting, network interface configuration, and a basic server setup, design, planning and organisation strategies.

## Functional test

### Router: Ubuntu Server

#### Network Configuration:
Command: sudo nano /etc/netplan/50-cloud-init.yaml

![network configuration-router](https://github.com/user-attachments/assets/9d8808ef-e121-4310-8415-cfbac0824fe1)

#### IP address of all adapters:
Command: ip a

![ip adapter](https://github.com/user-attachments/assets/e4846848-05e3-409a-920e-c047e2fbadaf)

#### Pinging Desktop VM and Application VM:

![ip adapter](https://github.com/user-attachments/assets/88e8a059-86ac-45ca-a04c-7094fe1c2400)

### Desktop VM: Ubuntu desktop
#### Setting up ip address:

![settingupip](https://github.com/user-attachments/assets/9feaf190-eea1-4d54-8d6d-fd463c98050e)

#### IP address of the adapter:
Command: ip a

![ipofall](https://github.com/user-attachments/assets/eb469b59-a26d-4af6-b20c-ae51769b0f0a)

#### Pinging to router:
Command: ping 10.0.2.15

![ping router](https://github.com/user-attachments/assets/f00e9d37-060c-4b9e-b4fa-f396637d6388)

#### Pinging to Application Server:
Command: ping 192.168.16.1

<img width="319" alt="ping to application" src="https://github.com/user-attachments/assets/0e96fcec-4d21-4330-8ceb-dfc72c293d1f">

### Application VM: Bitnami Wordpress
#### Network configuration:
Command: sudo nano /etc/network/interfaces

![netconf](https://github.com/user-attachments/assets/66c9d92a-13d3-48da-aef3-aa798ad7b8ab)

#### IP address of all adapters:
Command: ip a

![ipall](https://github.com/user-attachments/assets/66f12032-6a45-4617-acae-16dd5f73f415)

#### Pinging router:
Command: ping 10.0.2.15

![pr](https://github.com/user-attachments/assets/05cbdedd-2344-4e16-bf01-033649afe203)

#### Pinging Desktop VM:
Command: ping 192.168.116.1

![pdesk](https://github.com/user-attachments/assets/9b4bc3e6-206d-48fe-82ee-1751a97aeeab)






