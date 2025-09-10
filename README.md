# ArgoCD App of Apps repository.

ArgoCD in the OMF cluster gets its application definitions from this repository.
The app of apps is defined in the main terraform repository: https://github.com/OvertureMaps/omf-superset-opentofu/omf-argocd.tf 

## Description

This is using an ArgoCD ApplicationSet which automatically creates applications based on
the existance of a folder for the app under the deployments directory.

To create a new application to deploy to the omf eks cluster, add a folder under deployments with the application name and add
the pertinent yaml/charts etc, and ArgoCD will deploy what is contained therein.


