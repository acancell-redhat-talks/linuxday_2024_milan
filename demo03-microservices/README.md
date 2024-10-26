## CREDITS

As a microservice example, the project [Quarkus Super Heroes](https://github.com/quarkusio/quarkus-super-heroes) will be used.

## DEPLOY ON _OCP_

- `oc new-project quarkus-super-heroes`
- `oc apply -f https://raw.githubusercontent.com/quarkusio/quarkus-super-heroes/refs/heads/main/deploy/k8s/native-openshift.yml`
- `oc get route ui-super-heroes -o jsonpath='{"https://"}{.status.ingress[0].host}{"\n"}'`
