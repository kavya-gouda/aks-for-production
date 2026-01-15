# Kubernetes cert-manaher
- cert-manager is a native Kubernetes certificates Management controller
- It can help with issuing certificates from a variaty of sources, such a let's encrypt, Hashicorp vault, a vanafi, a simple signing pair or self signed
- It will ensure certificates are  valide until upto date, and attempt to renew certificates at a configured time before expiry
  
<img width="977" height="524" alt="image" src="https://github.com/user-attachments/assets/b58371fd-70e3-4f35-ae3f-7fa6d11372e4" />

- you will have cert-manager pod running in our cluster,
- you will have kubernetes secrets mounted to our ingress resources
- 
