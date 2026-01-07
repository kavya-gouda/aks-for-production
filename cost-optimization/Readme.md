## Reduce cost of AKS cluster

in kubernetes
- optimize Docker images
- Pod auto scalability(HPA)
- Nodes auto scalability (cluster autoscaler)

In AKS
- choose the right VM size
- Stop and Start cluster or nodepools
- Free and standard SKU for control plane
In Azure
- ARM vs intel based processors
- Azure Spot VM's(up to 80% of cost reduction
- Azure Reservations( 1 or 3 year)
- Azure Saving plan(up to 65 % off PAYG)
- Azure Hybrid Benefits(for windows server)
- Azure Dev/Test Subscriptions (no SLA)

## How much does an AKS cost?
Aks Cost includes
- VMSS (system & user)
- Load Balancer and IP adresses
- Network traffic between Zones
- Standard/premium SKU for the control plain
- Private Endpoint traffic if you are using private cluster

What is free in ASK
- the Control Plain
- Managed identity
- AKS extensions (OSM, CSI, drivers)

other cost:
- VNET peering with hub Network
- Application Gateway as ingress contrller
- Azure Keyvault for storing secrets and certifications
- Logs and Metrics: log analysis, prometheus and grafana
- persistent volumes using Azure disks, Blob or Files
- Cost of cluster Backup

# Technique to reduce the cost of aks cluster

1. Stop & start cluster (control plane and all worker node)
   could run as part of the Devops
   stop all the cluster nodes during non-working hours(weekend , nights)
   suited more the Dev/Test clusters, not recommended for production clusters
   save the cost of nodepools only, not other resources like Load Balancer, public ip
   <img width="1132" height="287" alt="image" src="https://github.com/user-attachments/assets/edaff88a-1548-4f19-974b-2889f86b6475" />

2. Stop & start nodepools
   <img width="1082" height="610" alt="image" src="https://github.com/user-attachments/assets/3ed8d0d4-92e2-4e43-ba3d-b2312f9fae67" />
3. choose the right size of VM SKU/family
   <img width="1142" height="541" alt="image" src="https://github.com/user-attachments/assets/4a2312d9-daa3-4b10-8090-4cffc2a5ab02" />
4. Autoscal the nodepools
   <img width="1047" height="569" alt="image" src="https://github.com/user-attachments/assets/4c1d1488-a644-4cae-bcae-663e68024835" />
5. Free vs Standard control plane SKU
   Free / standard control plane SKU 

- 
- 
- 
