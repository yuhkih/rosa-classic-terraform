# Terraform scripts for ROSA Classic

## Memos: 
- The default configuration of this terraform scrpit is 2 worker nodes in Single AZ. (defined in variables.tf)
- Single AZ or Multi AZ is determined by resource "rhcs_cluster_rosa_classic" in main.tf
- Need at least 5 worker nodes to host RHOAM.
- Need to export RHCL_TOKEN before start
If you already logged in to OCM, the following command works.
 ```
 export RHCS_TOKEN="$(jq -r .refresh_token ~/.config/ocm/ocm.json)
```
