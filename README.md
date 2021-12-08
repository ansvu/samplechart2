# samplechart2
Sample Chart 2
```diff
+ helm repo add samplechart  https://ansvu.github.io/samplechart
"samplechart" has been added to your repositories

+ helm repo list
NAME                            URL                                       
samplechart2                    https://ansvu.github.io/samplechart2   

+ helm install samplechart2 -n ava samplechart2/samplechart
NAME: samplechart2
LAST DEPLOYED: Tue Dec  7 22:43:57 2021
NAMESPACE: ava
STATUS: deployed
REVISION: 1
TEST SUITE: None
NOTES:

+ ka get po
NAME                            READY   STATUS    RESTARTS   AGE
samplechart2-76fc59d6f6-xspqg   1/1     Running   0          52s
```
- index.yaml
```yaml
apiVersion: v1
entries:
  samplechart:
  - annotations:
      charts.openshift.io/archs: x86_64
      charts.openshift.io/name: RedHat Test
      charts.openshift.io/provider: RedHat
      charts.openshift.io/supportURL: https://github.com/dperaza4dustbit/helm-chart
    apiVersion: v2
    appVersion: 1-42
    created: "2021-12-07T16:02:33.895292598-06:00"
    description: A Helm chart for Kubernetes
    digest: 22e56280264b02562e7c82c6a224bad6386e8bdd4bc7c7504ab8f92bbb46bc66
    icon: https://www.example.com/chart-icon.png
    kubeVersion: '>=1.20.0'
    name: samplechart
    urls:
    - https://github.com/ansvu/samplechart2/releases/download/samplechart-0.1.2/samplechart-0.1.2.tgz
    version: 0.1.2
generated: "2021-12-07T16:02:33.591365234-06:00"
```
