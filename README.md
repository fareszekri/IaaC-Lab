# IaaC-Lab
1. create an Azure vault to store your secrets :
`az keyvault create -n IaaCvault -g DevOps -l westeurope --enabled-for-deployment true  --enabled-for-template-deployment true`
2. Create your ssh_key secret : `az keyvault secret set -n sshkey --vault-name IaaCvault -f ~/.ssh/id_rsa.pub`
3. Link your keyvault to vsts : ![Link KeyVault](./images/linkKeyvault.gif)
4. Create your release to deploy your vm to Azure :






