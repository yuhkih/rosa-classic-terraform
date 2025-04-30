# Terraform scripts for ROSA Classic

## Memos: 
- Need at least 5 worker nodes to host RHOAM.
- Need to export RHCL_TOKEN before start
If you already logged in to OCM, the following command works.
 ```
 export RHCS_TOKEN="$(jq -r .refresh_token ~/.config/ocm/ocm.json)
```
