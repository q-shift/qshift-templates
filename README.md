# Backstage templates

- Templates to be used on a local Kubernetes cluster. See instructions [here](https://github.com/ch007m/package-backstage)
- Quarkus templates developed for the initiative QShift:
  - [Quarkus-application](qshift/templates/quarkus-application)
    This template allows to scaffold a Quarkus application using `code.quarkus.io` and to enrich the project with `starter` code. If you select as database `postgresql` and
    the extensions: `RESTeasy reactive`, `RESTeasy reactive jackson`, `REST resources for Hibernate ORM with Panache`, then the Quarkus application deployed on the Openshift cluster
    will access a local Postgresql DB to store some `My-entity` records. You will be abkle to access the application using the route: `https://my-quarkus-app-native-deploy-quarkus-deploy-<NAMESPACE>.<OCP_DOMAIN_NAME>/my-entity`
    
    **Important**: The recommendation is to delete the PVC of the postgres DB after played with a project scaffolded as the PVC
    is not deleted OOTB when we remove the ArgoCD Application installing the DB using Bitnami Helm chart. If you dont do that, as the generated password
    to access the DB changes, then you will get an authentication issue !

  - Quarkus-quickstart: Not up to date !!
