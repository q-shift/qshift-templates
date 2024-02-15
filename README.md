# Backstage templates

- Templates to be used on a local Kubernetes cluster. See instructions [here](https://github.com/ch007m/package-backstage)
- Quarkus templates developed for the initiative QShift:
  - [Quarkus-application](qshift/templates/quarkus-application)
    **Important**: The recommendation is to delete the PVC of the postgres DB end of the process to scaffold a quarkus application 
    as it is not deleted OOTB when we remove the ArgoCD Application installing the DB using Bitnami Helm chart
  - Quarkus-quickstart: Not up to date !!