# Backstage templates

- Templates to be used on a local Kubernetes cluster. See instructions [here](https://github.com/ch007m/package-backstage)
- Quarkus templates developed for the initiative QShift:
  - [Quarkus-application](qshift/templates/quarkus-application)
    
    **Important**: The recommendation is to delete the PVC of the postgres DB after played with a project scaffolded as the PVC
    is not deleted OOTB when we remove the ArgoCD Application installing the DB using Bitnami Helm chart. If you dont do that, as the generated password
    to access the DB changes, then you will get an authentication issue !

  - Quarkus-quickstart: Not up to date !!
