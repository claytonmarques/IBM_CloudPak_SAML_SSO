# Introdução

A configuração foi realizada sobre o IBM Cloud Pak Foundational Services versão 3.16 hospedado em IBM ROKS

Para verificar a versão do IBM Cloud Pak Foundational Services instalada no seu cluster, execute:
```
oc -n kube-public get ConfigMap ibmcloud-cluster-info -o jsonpath=’{.data.version}’ 
oc get csv --all-namespaces | grep common-service-
```

Para configura SSO, segui as instruções em:
https://www.ibm.com/docs/en/cpfs?topic=users-configuring-single-sign

Para instalar o cloudctl CLI:
https://www.ibm.com/docs/en/cpfs?topic=mycc-installing-cloudctl#curl

Para fazer o login no cluster com cloudctl
https://www.ibm.com/docs/en/cpfs?topic=operator-accessing-cluster-console

use o usuário admin (cloudctl não suporta IBMIDs).

IDP SAML https://samltest.id/

