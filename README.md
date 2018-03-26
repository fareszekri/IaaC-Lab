# IaaC-Lab
1 - create an Azure vault to store your secrets :
`az keyvault create -n IaaCvault -g DevOps -l westeurope --enabled-for-deployment true  --enabled-for-template-deployment true`

2 - Create your ssh_key secret : `az keyvault secret set -n sshkey --vault-name IaaCvault -f ~/.ssh/id_rsa.pub`




