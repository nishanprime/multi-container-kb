<code>Kubectl describe</code> outpus:

<code>
nishanthapa@Nishans-MacBook-Air multi-docker-prod % kb describe pods
Name:         client-deployment-7cb6c958f7-5zv5j
Namespace:    default
Priority:     0
Node:         docker-desktop/192.168.65.4
Start Time:   Mon, 28 Feb 2022 17:21:38 -0500
Labels:       component=web
              pod-template-hash=7cb6c958f7
Annotations:  <none>
Status:       Running
IP:           10.1.0.85
IPs:
  IP:           10.1.0.85
Controlled By:  ReplicaSet/client-deployment-7cb6c958f7
Containers:
  client:
    Container ID:   docker://52e7c80920a4ea7e97886e611c3e9a427efc865bc16692c8cff17e46ed091fc1
    Image:          stephengrider/multi-client
    Image ID:       docker-pullable://stephengrider/multi-client@sha256:855452509d6d9f13dbe1cd34fa3a21d7f6e7d1f0fafb38d1e715dda8e3d17f46
    Port:           3000/TCP
    Host Port:      0/TCP
    State:          Running
      Started:      Mon, 28 Feb 2022 17:21:40 -0500
    Ready:          True
    Restart Count:  0
    Environment:    <none>
    Mounts:
      /var/run/secrets/kubernetes.io/serviceaccount from kube-api-access-vkctr (ro)
Conditions:
  Type              Status
  Initialized       True 
  Ready             True 
  ContainersReady   True 
  PodScheduled      True 
Volumes:
  kube-api-access-vkctr:
    Type:                    Projected (a volume that contains injected data from multiple sources)
    TokenExpirationSeconds:  3607
    ConfigMapName:           kube-root-ca.crt
    ConfigMapOptional:       <nil>
    DownwardAPI:             true
QoS Class:                   BestEffort
Node-Selectors:              <none>
Tolerations:                 node.kubernetes.io/not-ready:NoExecute op=Exists for 300s
                             node.kubernetes.io/unreachable:NoExecute op=Exists for 300s
Events:
  Type    Reason     Age    From               Message
  ----    ------     ----   ----               -------
  Normal  Scheduled  3m     default-scheduler  Successfully assigned default/client-deployment-7cb6c958f7-5zv5j to docker-desktop
  Normal  Pulling    2m59s  kubelet            Pulling image "stephengrider/multi-client"
  Normal  Pulled     2m58s  kubelet            Successfully pulled image "stephengrider/multi-client" in 805.566333ms
  Normal  Created    2m58s  kubelet            Created container client
  Normal  Started    2m58s  kubelet            Started container client


Name:         client-deployment-7cb6c958f7-d5c5f
Namespace:    default
Priority:     0
Node:         docker-desktop/192.168.65.4
Start Time:   Mon, 28 Feb 2022 17:21:38 -0500
Labels:       component=web
              pod-template-hash=7cb6c958f7
Annotations:  <none>
Status:       Running
IP:           10.1.0.84
IPs:
  IP:           10.1.0.84
Controlled By:  ReplicaSet/client-deployment-7cb6c958f7
Containers:
  client:
    Container ID:   docker://c850573e8827cf7aeeb304baf06386a0c0c1eac4bab128de86d6cec5ac2ce9e3
    Image:          stephengrider/multi-client
    Image ID:       docker-pullable://stephengrider/multi-client@sha256:855452509d6d9f13dbe1cd34fa3a21d7f6e7d1f0fafb38d1e715dda8e3d17f46
    Port:           3000/TCP
    Host Port:      0/TCP
    State:          Running
      Started:      Mon, 28 Feb 2022 17:21:40 -0500
    Ready:          True
    Restart Count:  0
    Environment:    <none>
    Mounts:
      /var/run/secrets/kubernetes.io/serviceaccount from kube-api-access-574hs (ro)
Conditions:
  Type              Status
  Initialized       True 
  Ready             True 
  ContainersReady   True 
  PodScheduled      True 
Volumes:
  kube-api-access-574hs:
    Type:                    Projected (a volume that contains injected data from multiple sources)
    TokenExpirationSeconds:  3607
    ConfigMapName:           kube-root-ca.crt
    ConfigMapOptional:       <nil>
    DownwardAPI:             true
QoS Class:                   BestEffort
Node-Selectors:              <none>
Tolerations:                 node.kubernetes.io/not-ready:NoExecute op=Exists for 300s
                             node.kubernetes.io/unreachable:NoExecute op=Exists for 300s
Events:
  Type    Reason     Age    From               Message
  ----    ------     ----   ----               -------
  Normal  Scheduled  3m     default-scheduler  Successfully assigned default/client-deployment-7cb6c958f7-d5c5f to docker-desktop
  Normal  Pulling    2m59s  kubelet            Pulling image "stephengrider/multi-client"
  Normal  Pulled     2m59s  kubelet            Successfully pulled image "stephengrider/multi-client" in 662.310376ms
  Normal  Created    2m59s  kubelet            Created container client
  Normal  Started    2m58s  kubelet            Started container client


Name:         client-deployment-7cb6c958f7-jcd6k
Namespace:    default
Priority:     0
Node:         docker-desktop/192.168.65.4
Start Time:   Mon, 28 Feb 2022 17:21:38 -0500
Labels:       component=web
              pod-template-hash=7cb6c958f7
Annotations:  <none>
Status:       Running
IP:           10.1.0.83
IPs:
  IP:           10.1.0.83
Controlled By:  ReplicaSet/client-deployment-7cb6c958f7
Containers:
  client:
    Container ID:   docker://4e5fd99eff36bfdbe0f8a4bb1a52fdcc5b60058e29159afd5407f59091ed95c5
    Image:          stephengrider/multi-client
    Image ID:       docker-pullable://stephengrider/multi-client@sha256:855452509d6d9f13dbe1cd34fa3a21d7f6e7d1f0fafb38d1e715dda8e3d17f46
    Port:           3000/TCP
    Host Port:      0/TCP
    State:          Running
      Started:      Mon, 28 Feb 2022 17:21:39 -0500
    Ready:          True
    Restart Count:  0
    Environment:    <none>
    Mounts:
      /var/run/secrets/kubernetes.io/serviceaccount from kube-api-access-pn6gf (ro)
Conditions:
  Type              Status
  Initialized       True 
  Ready             True 
  ContainersReady   True 
  PodScheduled      True 
Volumes:
  kube-api-access-pn6gf:
    Type:                    Projected (a volume that contains injected data from multiple sources)
    TokenExpirationSeconds:  3607
    ConfigMapName:           kube-root-ca.crt
    ConfigMapOptional:       <nil>
    DownwardAPI:             true
QoS Class:                   BestEffort
Node-Selectors:              <none>
Tolerations:                 node.kubernetes.io/not-ready:NoExecute op=Exists for 300s
                             node.kubernetes.io/unreachable:NoExecute op=Exists for 300s
Events:
  Type    Reason     Age    From               Message
  ----    ------     ----   ----               -------
  Normal  Scheduled  3m     default-scheduler  Successfully assigned default/client-deployment-7cb6c958f7-jcd6k to docker-desktop
  Normal  Pulling    2m59s  kubelet            Pulling image "stephengrider/multi-client"
  Normal  Pulled     2m59s  kubelet            Successfully pulled image "stephengrider/multi-client" in 378.911042ms
  Normal  Created    2m59s  kubelet            Created container client
  Normal  Started    2m59s  kubelet            Started container client


Name:         postgres-deployment-5b7fdb4969-6vkdb
Namespace:    default
Priority:     0
Node:         docker-desktop/192.168.65.4
Start Time:   Mon, 28 Feb 2022 17:21:39 -0500
Labels:       component=postgres
              pod-template-hash=5b7fdb4969
Annotations:  <none>
Status:       Running
IP:           10.1.0.91
IPs:
  IP:           10.1.0.91
Controlled By:  ReplicaSet/postgres-deployment-5b7fdb4969
Containers:
  postgres:
    Container ID:   docker://b1db07f3335e607f2090009fc64f90ea36688be6f2a9d8225323e1cec7e66b7f
    Image:          postgres
    Image ID:       docker-pullable://postgres@sha256:156c50d4b6fe6ea4e4645ccdeabf54fedc59a561bfece047cdf4c26a42deab72
    Port:           5432/TCP
    Host Port:      0/TCP
    State:          Running
      Started:      Mon, 28 Feb 2022 17:21:43 -0500
    Ready:          True
    Restart Count:  0
    Environment:
      POSTGRES_PASSWORD:  <set to the key 'PGPASSWORD' in secret 'pgpassword'>  Optional: false
    Mounts:
      /var/lib/postgresql/data from postgres-storage (rw,path="postgres")
      /var/run/secrets/kubernetes.io/serviceaccount from kube-api-access-tx246 (ro)
Conditions:
  Type              Status
  Initialized       True 
  Ready             True 
  ContainersReady   True 
  PodScheduled      True 
Volumes:
  postgres-storage:
    Type:       PersistentVolumeClaim (a reference to a PersistentVolumeClaim in the same namespace)
    ClaimName:  database-persistent-volume-claim
    ReadOnly:   false
  kube-api-access-tx246:
    Type:                    Projected (a volume that contains injected data from multiple sources)
    TokenExpirationSeconds:  3607
    ConfigMapName:           kube-root-ca.crt
    ConfigMapOptional:       <nil>
    DownwardAPI:             true
QoS Class:                   BestEffort
Node-Selectors:              <none>
Tolerations:                 node.kubernetes.io/not-ready:NoExecute op=Exists for 300s
                             node.kubernetes.io/unreachable:NoExecute op=Exists for 300s
Events:
  Type     Reason            Age    From               Message
  ----     ------            ----   ----               -------
  Warning  FailedScheduling  3m     default-scheduler  0/1 nodes are available: 1 pod has unbound immediate PersistentVolumeClaims.
  Normal   Scheduled         2m59s  default-scheduler  Successfully assigned default/postgres-deployment-5b7fdb4969-6vkdb to docker-desktop
  Normal   Pulling           2m56s  kubelet            Pulling image "postgres"
  Normal   Pulled            2m56s  kubelet            Successfully pulled image "postgres" in 335.081917ms
  Normal   Created           2m56s  kubelet            Created container postgres
  Normal   Started           2m55s  kubelet            Started container postgres


Name:         redis-deployment-58c4799ccc-km82b
Namespace:    default
Priority:     0
Node:         docker-desktop/192.168.65.4
Start Time:   Mon, 28 Feb 2022 17:21:38 -0500
Labels:       component=redis
              pod-template-hash=58c4799ccc
Annotations:  <none>
Status:       Running
IP:           10.1.0.86
IPs:
  IP:           10.1.0.86
Controlled By:  ReplicaSet/redis-deployment-58c4799ccc
Containers:
  redis:
    Container ID:   docker://a8898f8dda2f1e96ba23568539d9732bc17b5129b15314ab3342265902cdca7c
    Image:          redis
    Image ID:       docker-pullable://redis@sha256:0d9c9aed1eb385336db0bc9b976b6b49774aee3d2b9c2788a0d0d9e239986cb3
    Port:           6379/TCP
    Host Port:      0/TCP
    State:          Running
      Started:      Mon, 28 Feb 2022 17:21:40 -0500
    Ready:          True
    Restart Count:  0
    Environment:    <none>
    Mounts:
      /var/run/secrets/kubernetes.io/serviceaccount from kube-api-access-2wr66 (ro)
Conditions:
  Type              Status
  Initialized       True 
  Ready             True 
  ContainersReady   True 
  PodScheduled      True 
Volumes:
  kube-api-access-2wr66:
    Type:                    Projected (a volume that contains injected data from multiple sources)
    TokenExpirationSeconds:  3607
    ConfigMapName:           kube-root-ca.crt
    ConfigMapOptional:       <nil>
    DownwardAPI:             true
QoS Class:                   BestEffort
Node-Selectors:              <none>
Tolerations:                 node.kubernetes.io/not-ready:NoExecute op=Exists for 300s
                             node.kubernetes.io/unreachable:NoExecute op=Exists for 300s
Events:
  Type    Reason     Age    From               Message
  ----    ------     ----   ----               -------
  Normal  Scheduled  3m     default-scheduler  Successfully assigned default/redis-deployment-58c4799ccc-km82b to docker-desktop
  Normal  Pulling    2m59s  kubelet            Pulling image "redis"
  Normal  Pulled     2m58s  kubelet            Successfully pulled image "redis" in 696.843ms
  Normal  Created    2m58s  kubelet            Created container redis
  Normal  Started    2m58s  kubelet            Started container redis


Name:         server-deployment-58cf857974-kfxcd
Namespace:    default
Priority:     0
Node:         docker-desktop/192.168.65.4
Start Time:   Mon, 28 Feb 2022 17:21:38 -0500
Labels:       component=server
              pod-template-hash=58cf857974
Annotations:  <none>
Status:       Running
IP:           10.1.0.90
IPs:
  IP:           10.1.0.90
Controlled By:  ReplicaSet/server-deployment-58cf857974
Containers:
  server:
    Container ID:   docker://d88d8c1f2e3660aae0057aa79726f4b6fa8881f3aa697e14c54cad14af2f26bf
    Image:          cygnetops/multi-server-pgfix-5-11
    Image ID:       docker-pullable://cygnetops/multi-server-pgfix-5-11@sha256:e605f0da73915e839477782a9952c39bac3581d8863384f26abfa0f42ad9d87d
    Port:           5000/TCP
    Host Port:      0/TCP
    State:          Running
      Started:      Mon, 28 Feb 2022 17:21:42 -0500
    Ready:          True
    Restart Count:  0
    Environment:
      REDIS_HOST:  redis-cluster-ip-service
      REDIS_PORT:  6379
      PGUSER:      postgres
      PGHOST:      postgres-cluster-ip-service
      PGPORT:      5432
      PGDATABASE:  postgres
      PGPASSWORD:  <set to the key 'PGPASSWORD' in secret 'pgpassword'>  Optional: false
    Mounts:
      /var/run/secrets/kubernetes.io/serviceaccount from kube-api-access-nxn7m (ro)
Conditions:
  Type              Status
  Initialized       True 
  Ready             True 
  ContainersReady   True 
  PodScheduled      True 
Volumes:
  kube-api-access-nxn7m:
    Type:                    Projected (a volume that contains injected data from multiple sources)
    TokenExpirationSeconds:  3607
    ConfigMapName:           kube-root-ca.crt
    ConfigMapOptional:       <nil>
    DownwardAPI:             true
QoS Class:                   BestEffort
Node-Selectors:              <none>
Tolerations:                 node.kubernetes.io/not-ready:NoExecute op=Exists for 300s
                             node.kubernetes.io/unreachable:NoExecute op=Exists for 300s
Events:
  Type    Reason     Age    From               Message
  ----    ------     ----   ----               -------
  Normal  Scheduled  3m     default-scheduler  Successfully assigned default/server-deployment-58cf857974-kfxcd to docker-desktop
  Normal  Pulling    2m57s  kubelet            Pulling image "cygnetops/multi-server-pgfix-5-11"
  Normal  Pulled     2m56s  kubelet            Successfully pulled image "cygnetops/multi-server-pgfix-5-11" in 626.214375ms
  Normal  Created    2m56s  kubelet            Created container server
  Normal  Started    2m56s  kubelet            Started container server


Name:         server-deployment-58cf857974-qdhbq
Namespace:    default
Priority:     0
Node:         docker-desktop/192.168.65.4
Start Time:   Mon, 28 Feb 2022 17:21:38 -0500
Labels:       component=server
              pod-template-hash=58cf857974
Annotations:  <none>
Status:       Running
IP:           10.1.0.88
IPs:
  IP:           10.1.0.88
Controlled By:  ReplicaSet/server-deployment-58cf857974
Containers:
  server:
    Container ID:   docker://5ad7339197e9cb1c653e360cbf2fbb7a4cc1a72e1c9b306f7d75a8f390bdc674
    Image:          cygnetops/multi-server-pgfix-5-11
    Image ID:       docker-pullable://cygnetops/multi-server-pgfix-5-11@sha256:e605f0da73915e839477782a9952c39bac3581d8863384f26abfa0f42ad9d87d
    Port:           5000/TCP
    Host Port:      0/TCP
    State:          Running
      Started:      Mon, 28 Feb 2022 17:21:41 -0500
    Ready:          True
    Restart Count:  0
    Environment:
      REDIS_HOST:  redis-cluster-ip-service
      REDIS_PORT:  6379
      PGUSER:      postgres
      PGHOST:      postgres-cluster-ip-service
      PGPORT:      5432
      PGDATABASE:  postgres
      PGPASSWORD:  <set to the key 'PGPASSWORD' in secret 'pgpassword'>  Optional: false
    Mounts:
      /var/run/secrets/kubernetes.io/serviceaccount from kube-api-access-8tvf6 (ro)
Conditions:
  Type              Status
  Initialized       True 
  Ready             True 
  ContainersReady   True 
  PodScheduled      True 
Volumes:
  kube-api-access-8tvf6:
    Type:                    Projected (a volume that contains injected data from multiple sources)
    TokenExpirationSeconds:  3607
    ConfigMapName:           kube-root-ca.crt
    ConfigMapOptional:       <nil>
    DownwardAPI:             true
QoS Class:                   BestEffort
Node-Selectors:              <none>
Tolerations:                 node.kubernetes.io/not-ready:NoExecute op=Exists for 300s
                             node.kubernetes.io/unreachable:NoExecute op=Exists for 300s
Events:
  Type    Reason     Age    From               Message
  ----    ------     ----   ----               -------
  Normal  Scheduled  3m     default-scheduler  Successfully assigned default/server-deployment-58cf857974-qdhbq to docker-desktop
  Normal  Pulling    2m57s  kubelet            Pulling image "cygnetops/multi-server-pgfix-5-11"
  Normal  Pulled     2m57s  kubelet            Successfully pulled image "cygnetops/multi-server-pgfix-5-11" in 358.340083ms
  Normal  Created    2m57s  kubelet            Created container server
  Normal  Started    2m57s  kubelet            Started container server


Name:         server-deployment-58cf857974-vh9kb
Namespace:    default
Priority:     0
Node:         docker-desktop/192.168.65.4
Start Time:   Mon, 28 Feb 2022 17:21:38 -0500
Labels:       component=server
              pod-template-hash=58cf857974
Annotations:  <none>
Status:       Running
IP:           10.1.0.87
IPs:
  IP:           10.1.0.87
Controlled By:  ReplicaSet/server-deployment-58cf857974
Containers:
  server:
    Container ID:   docker://07386d5fc4a725c983e3aa21d0a0cd59098339d7fb76cd5543a582ce216db257
    Image:          cygnetops/multi-server-pgfix-5-11
    Image ID:       docker-pullable://cygnetops/multi-server-pgfix-5-11@sha256:e605f0da73915e839477782a9952c39bac3581d8863384f26abfa0f42ad9d87d
    Port:           5000/TCP
    Host Port:      0/TCP
    State:          Running
      Started:      Mon, 28 Feb 2022 17:21:41 -0500
    Ready:          True
    Restart Count:  0
    Environment:
      REDIS_HOST:  redis-cluster-ip-service
      REDIS_PORT:  6379
      PGUSER:      postgres
      PGHOST:      postgres-cluster-ip-service
      PGPORT:      5432
      PGDATABASE:  postgres
      PGPASSWORD:  <set to the key 'PGPASSWORD' in secret 'pgpassword'>  Optional: false
    Mounts:
      /var/run/secrets/kubernetes.io/serviceaccount from kube-api-access-r7vdp (ro)
Conditions:
  Type              Status
  Initialized       True 
  Ready             True 
  ContainersReady   True 
  PodScheduled      True 
Volumes:
  kube-api-access-r7vdp:
    Type:                    Projected (a volume that contains injected data from multiple sources)
    TokenExpirationSeconds:  3607
    ConfigMapName:           kube-root-ca.crt
    ConfigMapOptional:       <nil>
    DownwardAPI:             true
QoS Class:                   BestEffort
Node-Selectors:              <none>
Tolerations:                 node.kubernetes.io/not-ready:NoExecute op=Exists for 300s
                             node.kubernetes.io/unreachable:NoExecute op=Exists for 300s
Events:
  Type    Reason     Age    From               Message
  ----    ------     ----   ----               -------
  Normal  Scheduled  3m     default-scheduler  Successfully assigned default/server-deployment-58cf857974-vh9kb to docker-desktop
  Normal  Pulling    2m58s  kubelet            Pulling image "cygnetops/multi-server-pgfix-5-11"
  Normal  Pulled     2m57s  kubelet            Successfully pulled image "cygnetops/multi-server-pgfix-5-11" in 532.233417ms
  Normal  Created    2m57s  kubelet            Created container server
  Normal  Started    2m57s  kubelet            Started container server


Name:         worker-deployment-7c94ff9b64-8h6m2
Namespace:    default
Priority:     0
Node:         docker-desktop/192.168.65.4
Start Time:   Mon, 28 Feb 2022 17:21:38 -0500
Labels:       component=worker
              pod-template-hash=7c94ff9b64
Annotations:  <none>
Status:       Running
IP:           10.1.0.89
IPs:
  IP:           10.1.0.89
Controlled By:  ReplicaSet/worker-deployment-7c94ff9b64
Containers:
  worker:
    Container ID:   docker://ab6961c7aa8ca18a710f9b2879b9d07170a6e9a85e2b7a290b0b124145f65ead
    Image:          stephengrider/multi-worker
    Image ID:       docker-pullable://stephengrider/multi-worker@sha256:5fbab5f86e6a4d499926349a5f0ec032c42e7f7450acc98b053791df26dc4d2b
    Port:           <none>
    Host Port:      <none>
    State:          Running
      Started:      Mon, 28 Feb 2022 17:21:41 -0500
    Ready:          True
    Restart Count:  0
    Environment:
      REDIS_HOST:  redis-cluster-ip-service
      REDIS_PORT:  6379
    Mounts:
      /var/run/secrets/kubernetes.io/serviceaccount from kube-api-access-5hx6n (ro)
Conditions:
  Type              Status
  Initialized       True 
  Ready             True 
  ContainersReady   True 
  PodScheduled      True 
Volumes:
  kube-api-access-5hx6n:
    Type:                    Projected (a volume that contains injected data from multiple sources)
    TokenExpirationSeconds:  3607
    ConfigMapName:           kube-root-ca.crt
    ConfigMapOptional:       <nil>
    DownwardAPI:             true
QoS Class:                   BestEffort
Node-Selectors:              <none>
Tolerations:                 node.kubernetes.io/not-ready:NoExecute op=Exists for 300s
                             node.kubernetes.io/unreachable:NoExecute op=Exists for 300s
Events:
  Type    Reason     Age    From               Message
  ----    ------     ----   ----               -------
  Normal  Scheduled  3m     default-scheduler  Successfully assigned default/worker-deployment-7c94ff9b64-8h6m2 to docker-desktop
  Normal  Pulling    2m57s  kubelet            Pulling image "stephengrider/multi-worker"
  Normal  Pulled     2m57s  kubelet            Successfully pulled image "stephengrider/multi-worker" in 608.363583ms
  Normal  Created    2m57s  kubelet            Created container worker
  Normal  Started    2m57s  kubelet            Started container worker
nishanthapa@Nishans-MacBook-Air multi-docker-prod % 
</code>
  
 And:
  
  ingres service desribe logs are:
  
  <code>
  Name:             ingress-service
Namespace:        default
Address:          
Default backend:  default-http-backend:80 (<error: endpoints "default-http-backend" not found>)
Rules:
  Host        Path  Backends
  ----        ----  --------
  *           
              /?(.*)       client-cluster-ip-service:3000 (10.1.0.83:3000,10.1.0.84:3000,10.1.0.85:3000)
              /api/?(.*)   server-cluster-ip-service:5000 (10.1.0.87:5000,10.1.0.88:5000,10.1.0.90:5000)
Annotations:  kubernetes.io/ingress.class: nginx
              nginx.ingress.kubernetes.io/rewrite-target: /$1
              nginx.ingress.kubernetes.io/use-regex: true
Events:       <none>
nishanthapa@Nishans-MacBook-Air multi-docker-prod % 
  </code>
