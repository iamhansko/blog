
[추천 Udemy 강의](https://www.udemy.com/share/101WmE3@S_JJPisd9_H2eSP4ptgZqgGZ92a80XyDBBGpOJpeN4a4PrBEvzjMtOjYd5lkxoNQIg==/), 해당 강의를 구매하면 연습용 실습 환경과 문제+해설을 제공한다. 이 연습 문제들은 실제 시험 문제와 상당히 유사하다.

kubectl 명령어에 익숙해야만 시간 내에 문제 풀기 가능

![cka_cert](/img/cka_hyunsuko.png)

## 예상 문제유형
1. Upgrade **kubeadm**, **kubelet**, **kubectl**
1. Scale in/out Deployment 
    ```
    kubectl scale deployment --replicas=0 ...
    ```
1. Fix a Node (Not Ready -> Ready)
    ```
    sudo systemctl status kubelet
    sudo systemctl restart kubelet
    ```
1. Find 'Highest CPU Usage'
    ```
    kubectl top node
    kubectl top pod
    ```
1. Find # of Nodes affected/not_affected by Taint
1. Make a Node Not Ready, Not schedulable 
    ```
    kubectl drain ...
    kubectl cordon ...
    ```
1. ETCD Backup 
    ```
    etcdctl ...
    ```
1. Create a Pod
1. Create a Multi-Container Pod
    - Share emptyDir Volume using volumeMounts
1. Create a Deployment
1. Create a Service
1. Create an Ingress
1. Create PVC + Pod(volumeMounts + volume)
    ```
    kubectl edit storageclass ... 
    # ...
    # allowVolumeExpansion : true
    # ...
    ```
1. Create a PV
    - hostPath
1. Create ServiceAccount + Role + RoleBinding
1. Create a NetworkPolicy
    - podSelector
    - namespaceSelector
1. Logging
    ```
    kubect logs ... | grep ... > file.txt
    ```