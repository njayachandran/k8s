root@kube-master:~/k8s# cat HISTORY.txt                                                                                                                                                               
    1  git clone https://github.com/njayachandran/k8s                                                                                                                                                 
    2  ls                                                                                                                                                                                             
    3  cd k8s/                                                                                                                                                                                        
    4  cd 00-Setup/                                                                                                                                                                                   
    5  ls                                                                                                                                                                                             
    6  sh install-k8s-master-node.sh                                                                                                                                                                  
    7  hostname -i                                                                                                                                                                                    
    8  ls                                                                                                                                                                                             
    9  vim install-k8s-master-node.sh                                                                                                                                                                 
   10  sh install-k8s-master-node.sh                                                                                                                                                                  
   11  mkdir -p $HOME/.kube                                                                                                                                                                           
   12  sudo cp -i /etc/kubernetes/admin.conf /root/.kube/config                                                                                                                                       
   13  sudo chown $(id -u):$(id -u) $HOME/.kube/config                                                                                                                                                
   14  kubectl get ns                                                                                                                                                                                 
   15  kubectl get pods                                                                                                                                                                               
   16  kubectl get nodes                                                                                                                                                                              
   17  kubectl get nodes -o wide                                                                                                                                                                      
   18  cat $HOME/.kube/config                                                                                                                                                                         
   19  clear                                                                                                                                                                                          
   20  kubectl get nodes                                                                                                                                                                              
   21  kubectl get nodes -o wide                                                                                                                                                                      
   22  clear                                                                                                                                                                                          
   23  kubectl get nodes -o wide                                                                                                                                                                      
   24  kubeadm token list                                                                                                                                                                             
   25  ping google.com                                                                                                                                                                                
   26  kubeadm token create --print-join-command                                                                                                                                                      
   27  kubeadm token create --help                                                                                                                                                                    
   28  kubeadm token create --print-join-command --skip-log-headers                                                                                                                                   
   29  kubeadm token create --print-join-command -v=0                                                                                                                                                 
   30  kubeadm token create --print-join-command -v=1                                                                                                                                                 
   31  kubeadm token create --print-join-command --skip-headers                                                                                                                                       
   32  clear                                                                                                                                                                                          
   33  kubectl get pods -A                                                                                                                                                                            
   34  kubectl get ns                                                                                                                                                                                 
   35  kubectl run hello-k8s --image=nginx --port=80                                                                                                                                                  
   36  kubectl get pods                                                                                                                                                                               
   37  kubectl get pods -o wide                                                                                                                                                                       
   38  kubectl run hello-k8s-2 --image=gcr.io/google_containers/hpa-example --port=80                                                                                                                 
   39  kubectl get pods -o wide                                                                                                                                                                       
   40  kubectl get pods                                                                                                                                                                               
   41  kubectl descrive pods hello-k8s-2                                                                                                                                                              
   42  kubectl describe pods hello-k8s-2                                                                                                                                                              
   43  kubectl get pods                                                                                                                                                                               
   44  kubectl delete pods hello-k8s-2                                                                                                                                                                
   45  kubectl run hello-k8s-2 --image=gcr.io/google_containers/hpa-example --port=80                                                                                                                 
   46  kubectl describe pods                                                                                                                                                                          
   47  kunectl get pods                                                                                                                                                                               
   48  kubectl get pods                                                                                                                                                                               
   49  kubectl get pods -n kube-system                                                                                                                                                                
   50  kubectl exec -it etcd-kube-master -- /bin/sh                                                                                                                                                   
   51  kubectl exec -it etcd-kube-master -n kube-system -- /bin/sh                                                                                                                                    
   52  kubectl proxy                                                                                                                                                                                  
   53  kubectl proxy --address='172.31.0.10'                                                                                                                                                          
   54  kubectl proxy --address='172.31.0.10' --port=8001                                                                                                                                              
   55  kubectl proxy --address='172.31.0.10' --port=8001 --accept-hosts='.' --accept-paths='.'                                                                                                        
   56  kubectl proxy --address='172.31.0.10'                                                                                                                                                          
   57  kubectl proxy --address='172.31.0.10' --port=8001 --accept-hosts='.' --accept-paths='.'                                                                                                        
   58  kubectl config view                                                                                                                                                                            
   59  git pull                                                                                                                                                                                       
   60  cd ..                                                                                                                                                                                          
   61  /ls                                                                                                                                                                                            
   62  cd ../                                                                                                                                                                                         
   63  git clone https://github.com/amitvashisttech/k8s-paypal-28-Dec-2020                                                                                                                            
   64  ls                                                                                                                                                                                             
   65  cd k8s                                                                                                                                                                                         
   66  cd ../k8s-paypal-28-Dec-2020/                                                                                                                                                                  
   67  ls                                                                                                                                                                                             
   68  cd 04-ReplicationCantroller/                                                                                                                                                                   
   69  ls                                                                                                                                                                                             
   70  cat helloworld-rc.yaml                                                                                                                                                                         
   71  ls /root/.docker/config.js                                                                                                                                                                     
   72  ls ~/.docker/config.js                                                                                                                                                                         
   73  cd $HOME                                                                                                                                                                                       
   74  ls                                                                                                                                                                                             
   75  docker logout                                                                                                                                                                                  
   76  docker login                                                                                                                                                                                   
   77  ls                                                                                                                                                                                             
   78  cd .docker/                                                                                                                                                                                    
   79  ls                                                                                                                                                                                             
   80  cat config.json                                                                                                                                                                                
   81  kubectl create secret generic regcred --from-file=.dockerconfigjson=/root/.docker/config.js on --type=kubernetes.io/dockerconfigjson                                                           
   82  kubectl create secret regcred --from-file=.dockerconfigjson=/root/.docker/config.js on --type=kubernetes.io/dockerconfigjson                                                                   
   83  kubectl create secret generic regcred --from-file=.dockerconfigjson=/root/.docker/config.js on --type=kubernetes.io/dockerconfigjson                                                           
   84  kubectl create secret generic -h                                                                                                                                                               
   85  kubectl create secret generic regcred --from-file=.dockerconfigjson=.docker/config.js on --type=kubernetes.io/dockerconfigjson                                                                 
   86  'kubectl create secret generic -h                                                                                                                                                              
   87  kubectl create secret generic -h                                                                                                                                                               
   88  kubectl create secret generic regcred --from-file=.dockerconfigjson=.docker/config.json --type=kubernetes.io/dockerconfigjson                                                                  
   89  kubectl create secret generic regcred --from-file=.dockerconfigjson=/root/.docker/config.json --type=kubernetes.io/dockerconfigjson                                                            
   90  kubectl get secret                                                                                                                                                                             
   91  cd /root/                                                                                                                                                                                      
   92  ls                                                                                                                                                                                             
   93  cd k8s-paypal-28-Dec-2020/                                                                                                                                                                     
   94  ls                                                                                                                                                                                             
   95  cd 04-ReplicationCantroller/                                                                                                                                                                   
   96  ls                                                                                                                                                                                             
   97  cat helloworld-rc.yaml                                                                                                                                                                         
   98  kubectl apply -f helloworld-rc.yaml                                                                                                                                                            
   99  watch -n .5 kubectl get pods                                                                                                                                                                   
  100  kubectl get rc                                                                                                                                                                                 
  101  kubectl describe rc helloworld-container                                                                                                                                                       
  102  kubectl describe rc helloworld-controller                                                                                                                                                      
  103  cd ../../                                                                                                                                                                                      
  104  ls                                                                                                                                                                                             
  105  cd k8s-paypal-28-Dec-2020/                                                                                                                                                                     
  106  ls                                                                                                                                                                                             
  107  git pull                                                                                                                                                                                       
  108  ls                                                                                                                                                                                             
  109  cd 05-Deployments/                                                                                                                                                                             
  110  ls                                                                                                                                                                                             
  111  kubectl create -f helloworld.yaml                                                                                                                                                              
  112  kubectl get deploy,rs,pods                                                                                                                                                                     
  113  kubectl delete rc helloworld-controller                                                                                                                                                        
  114  kubectl get deploy,rs,pods                                                                                                                                                                     
  115  kubectl edit deploy helloworld-deploy                                                                                                                                                          
  116  kubectl edit deploy helloworld-deployment                                                                                                                                                      
  117  kubectl rollout history deploy helloworld-deployment                                                                                                                                           
  118  kubectl set image deploy helloworld-deployment k8s-demo=amitvashist7/k8s-tiny-web:3 --record                                                                                                   
  119  kubectl rollout history deploy helloworld-deployment                                                                                                                                           
  120  kubectl get deploy,rs,pods                                                                                                                                                                     
  121  kubectl scale --replicas=3 deploy helloworld-deployment                                                                                                                                        
  122  kubectl get deploy,rs,pods                                                                                                                                                                     
  123  kubectl scale --replicas=5 deploy helloworld-deployment --record                                                                                                                               
  124  kubectl get deploy,rs,pods                                                                                                                                                                     
  125  kubectl rollout history deploy helloworld-deployment                                                                                                                                           
  126  kubectl scale --replicas=3 deploy helloworld-deployment --record                                                                                                                               
  127  kubectl rollout history deploy helloworld-deployment                                                                                                                                           
  128  kubectl rollout undo deploy helloworld-deployment                                                                                                                                              
  129  kubectl rollout history deploy helloworld-deployment                                                                                                                                           
  130  kubectl rollout undo deploy helloworld-deployment                                                                                                                                              
  131  kubectl rollout history deploy helloworld-deployment                                                                                                                                           
  132  kubectl rollout history deploy helloworld-deployment --revision=1                                                                                                                              
  133  kubectl rollout history deploy helloworld-deployment --revision=2                                                                                                                              
  134  kubectl rollout history deploy helloworld-deployment --revision=4                                                                                                                              
  135  kubectl rollout history deploy helloworld-deployment --revision=5                                                                                                                              
  136  git pull                                                                                                                                                                                       
  137  ls                                                                                                                                                                                             
  138  vim helloworld-v3.yaml                                                                                                                                                                         
  139  kubectl delete -f helloworld.yaml                                                                                                                                                              
  140  kubectl get rs, deploy, pods                                                                                                                                                                   
  141  kubectl get rs,deploy,pods                                                                                                                                                                     
  142  kubectl delete pods hello-k8s                                                                                                                                                                  
  143  kubectl delete pods hello-k8s-2                                                                                                                                                                
  144  kubectl create -f helloworld-v2.yaml --record                                                                                                                                                  
  145  kubectl get deploy,rs,pods                                                                                                                                                                     
  146  kubectl rollout status deploy helloworld-2-deployment                                                                                                                                          
  147  kubectl rollout history deploy helloworld-2-deployment                                                                                                                                         
  148  kubectl rollout history deploy helloworld-2-deployment --revision=1                                                                                                                            
  149  kubectl set image deploy helloworld-2-deployment k8s-demo=amitvashist7/k8s-tiny-web:2 --record                                                                                                 
  150  kubectl rollout history deploy helloworld-2-deployment                                                                                                                                         
  151  kubectl get deploy,rs,pods                                                                                                                                                                     
  152  kubectl rollout history deploy helloworld-2-deployment                                                                                                                                         
  153  kubectl delete -f helloworld-v2.yaml                                                                                                                                                           
  154  kubectl get deploy,rs,pods                                                                                                                                                                     
  155  kubectl create -f helloworld-v3.yaml                                                                                                                                                           
  156  kubectl delete -f helloworld-v2.yaml                                                                                                                                                           
  157  kubectl get deploy,rs,pods                                                                                                                                                                     
  158  kubectl set image deploy helloworld-3-deployment k8s-demo=amitvashist7/k8s-tiny-web:2 --record                                                                                                 
  159  kubectl get deploy,rs,pods                                                                                                                                                                     
  160  kubectl rollout pause deploy helloworld-3-deployment --record                                                                                                                                  
  161  kubectl rollout pause deploy helloworld-3-deployment                                                                                                                                           
  162  kubectl set image deploy helloworld-3-deployment k8s-demo=amitvashist7/k8s-tiny-web:3 --record                                                                                                 
  163  kubectl get deploy,rs,pods                                                                                                                                                                     
  164  kubectl rollout history deploy helloworld-3-deployment                                                                                                                                         
  165  kubectl rollout resume deploy helloworld-3-deployment                                                                                                                                          
  166  kubectl rollout history deploy helloworld-3-deployment                                                                                                                                         
  167  kubectl rollout status deploy helloworld-3-deployment                                                                                                                                          
  168  kubectl rollout history deploy helloworld-3-deployment                                                                                                                                         
  169  git pull                                                                                                                                                                                       
  170  cd ../06-Service/                                                                                                                                                                              
  171  ls                                                                                                                                                                                             
  172  cat helloworld.yaml                                                                                                                                                                            
  173  kubectl get deploy                                                                                                                                                                             
  174  kubectl delete deploy helloworld-3-deployment                                                                                                                                                  
  175  kubectl get pods                                                                                                                                                                               
  176  clear                                                                                                                                                                                          
  177  ls                                                                                                                                                                                             
  178  cat app-service.yaml                                                                                                                                                                           
  179  clear                                                                                                                                                                                          
  180  cat helloworld-svc.yaml                                                                                                                                                                        
  181  clear                                                                                                                                                                                          
  182  cat helloworld                                                                                                                                                                                 
  183  cat helloworld.yaml                                                                                                                                                                            
  184  kubectl apply -f helloworld.yaml                                                                                                                                                               
  185  kubectl get svc                                                                                                                                                                                
  186  kubectl get deploy                                                                                                                                                                             
  187  kubect status deploy helloworld-deployment                                                                                                                                                     
  188  kubectl status deploy helloworld-deployment                                                                                                                                                    
  189  kubectl rollout status deploy helloworld-deployment                                                                                                                                            
  190  kubectl get pods                                                                                                                                                                               
  191  kubectl get pods -o wide                                                                                                                                                                       
  192  kubectl get svc                                                                                                                                                                                
  193  kubectl apply -f helloworld-svc.yaml                                                                                                                                                           
  194  kubectl get svc                                                                                                                                                                                
  195  kubectl describe svc helloworld-service                                                                                                                                                        
  196  kubectl get api-version                                                                                                                                                                        
  197  kubectl api-version                                                                                                                                                                            
  198  kubectl api-versions                                                                                                                                                                           
  199  kubectl cluster-info                                                                                                                                                                           
  200  kubectl cluster-info dump                                                                                                                                                                      
  201  kubectl get svc                                                                                                                                                                                
  202  kubectl get pods                                                                                                                                                                               
  203  kubectl exec -it helloworld-deployment-78cf6987f9-6r245 -- /bin/sh                                                                                                                             
  204  kubectl get pods                                                                                                                                                                               
  205  kubectl exec -it helloworld-deployment-78cf6987f9-6r245 -- /bin/sh                                                                                                                             
  206  kubectl get pods -o wide                                                                                                                                                                       
  207  history | grep exec                                                                                                                                                                            
  208  kubectl get pods                                                                                                                                                                               
  209  kubectl exec -it helloworld-deployment-78cf6987f9-6r245 -- /bin/bash                                                                                                                           
  210  ls                                                                                                                                                                                             
  211  kubectl get deploy,rs,pods                                                                                                                                                                     
  212  kubectl get svc,deploy,rs,pods                                                                                                                                                                 
  213  kubectl exec -it helloworld-deployment -- /bin/sh                                                                                                                                              
  214  kubectl exec -it helloworld-deployment-78cf6987f9-6r245 -- /bin/sh                                                                                                                             
  215  kubectl exec -it helloworld-deployment-78cf6987f9-6r245 -- hostname -i                                                                                                                         
  216  kubectl exec -it kube-master -- hostname -i                                                                                                                                                    
  217  kubectl exec -it kube-master -n kube-system -- hostname -i                                                                                                                                     
  218  kubectl get pods -n kube-system                                                                                                                                                                
  219  kubectl exec -it etcd-kube-master -n kube-system -- /bin/sh                                                                                                                                    
  220  clear                                                                                                                                                                                          
  221  kubectl get svc                                                                                                                                                                                
  222  kubectl describe svc helloworld-service                                                                                                                                                        
  223  clear                                                                                                                                                                                          
  224  ls                                                                                                                                                                                             
  225  cat app-service.yaml                                                                                                                                                                           
  226  git pull                                                                                                                                                                                       
  227  cd ../07-HealthChecks/                                                                                                                                                                         
  228  kubectl get svc                                                                                                                                                                                
  229  kubectl delete -f ../06-Service/                                                                                                                                                               
  230  ls                                                                                                                                                                                             
  231  clear                                                                                                                                                                                          
  232  cat helloworld-deploy-http-healthcheck.yaml                                                                                                                                                    
  233  kubectl create -f helloworld-deploy-http-healthcheck.yaml                                                                                                                                      
  234  kubectl get deploy                                                                                                                                                                             
  235  kubectl get pods                                                                                                                                                                               
  236  kubectl get deploy                                                                                                                                                                             
  237  kubectl edit deploy helloworld-deployment                                                                                                                                                      
  238  kubectl get deploy                                                                                                                                                                             
  239  kubectl get deploy,pods                                                                                                                                                                        
  240  kubectl get deploy,rs,pods                                                                                                                                                                     
  241  kubectl describe pods pod/helloworld-deployment-75d4775f-6jm8w                                                                                                                                 
  242  kubectl describe pods helloworld-deployment-75d4775f-6jm8w                                                                                                                                     
  243  kubectl edit deploy helloworld-deployment                                                                                                                                                      
  244  kubectl get pods                                                                                                                                                                               
  245  kubectl describe pods helloworld-deployment-585fb455cb-t77kv                                                                                                                                   
  246  kubectl get pods                                                                                                                                                                               
  247  ls                                                                                                                                                                                             
  248  git pull                                                                                                                                                                                       
  249  kubectl delete -f                                                                                                                                                                              
  250  kubectl delete -f .                                                                                                                                                                            
  251  kubectl get pods                                                                                                                                                                               
  252  clear                                                                                                                                                                                          
  253  ls                                                                                                                                                                                             
  254  cat helloworld-deploy-custom-values.yaml                                                                                                                                                       
  255  kubectl create -f helloworld-deploy-custom-values.yaml                                                                                                                                         
  256  kubectl get deploy                                                                                                                                                                             
  257  kubectl describe deploy helloworld-deployment                                                                                                                                                  
  258  kubectl get deploy                                                                                                                                                                             
  259  kubectl get pods                                                                                                                                                                               
  260  kubectl describe pods helloworld-deployment-76476854c6-rwx5z                                                                                                                                   
  261  kubectl delete -f helloworld-deploy-custom-values.yaml                                                                                                                                         
  262  ls                                                                                                                                                                                             
  263  kubectl helloworld-deploy-http-healthcheck.yaml                                                                                                                                                
  264  kubectl create -f helloworld-deploy-http-healthcheck.yaml                                                                                                                                      
  265  kubectl get svc                                                                                                                                                                                
  266  kubectl get deploy                                                                                                                                                                             
  267  kubectl get pods                                                                                                                                                                               
  268  kubectl describe pods helloworld-deployment-585fb455cb-6lkrt                                                                                                                                   
  269  exit                                                                                                                                                                                           
  270  kubectl get svc                                                                                                                                                                                
  271  ls                                                                                                                                                                                             
  272  cd /root/                                                                                                                                                                                      
  273  ls                                                                                                                                                                                             
  274  cd k8s-paypal-28-Dec-2020/                                                                                                                                                                     
  275  ls                                                                                                                                                                                             
  276  cd 01-First-App/                                                                                                                                                                               
  277  ls                                                                                                                                                                                             
  278  cat README.md                                                                                                                                                                                  
  279  kubectl run hello-k8s --image=gcr.io/google_containers/hpa-example --port=80                                                                                                                   
  280  kubectl get pods                                                                                                                                                                               
  281  kubectl get pods -o wide                                                                                                                                                                       
  282  cd ../11-DNS/                                                                                                                                                                                  
  283  ls                                                                                                                                                                                             
  284  cat History.txt                                                                                                                                                                                
  285  clear                                                                                                                                                                                          
  286  kubectl create -f custom-dns.yaml                                                                                                                                                              
  287  kubectl get pods                                                                                                                                                                               
  288  kubectl exec -it custom-dns-example -- cat /etc/resolv.conf                                                                                                                                    
  289  kubectl exec -it busybox -- cat /etc/resolv.conf                                                                                                                                               
  290  kubectl get pods -o wide                                                                                                                                                                       
  291  cat History.txt                                                                                                                                                                                
  292  kubectl exec -it busybox -- cat /etc/resolv.conf                                                                                                                                               
  293  clear                                                                                                                                                                                          
  294  ls                                                                                                                                                                                             
  295  cat busybox-headless.yaml                                                                                                                                                                      
  296  kubectl apply -f busybox-headless.yaml                                                                                                                                                         
  297  kubectl get svc                                                                                                                                                                                
  298  clear                                                                                                                                                                                          
  299  kubectl get pods                                                                                                                                                                               
  300  kubectl exec -it custom-dns-example -- cat /etc/resolv.conf                                                                                                                                    
  301  kubectl get pods -o wide                                                                                                                                                                       
  302  kubectl edif configmap ngninx-config                                                                                                                                                           
  303  kubectl edit configmap ngninx-config                                                                                                                                                           
  304  kubectl get configmap                                                                                                                                                                          
  305  kubectl edit configmap nginx-config                                                                                                                                                            
  306  cd ../15-ResourceQuotas/                                                                                                                                                                       
  307  ls                                                                                                                                                                                             
  308  vim helloworld-with-quota.yaml                                                                                                                                                                 
  309  kubectl apply -f helloworld-with-quota.yaml                                                                                                                                                    
  310  kubectl get deploy -n myspace                                                                                                                                                                  
  311  kubectl get quota -n myspace                                                                                                                                                                   
  312  ls                                                                                                                                                                                             
  313  vim helloworld-with-quota.yaml                                                                                                                                                                 
  314  kubectl apply -f helloworld-with-quota.yaml                                                                                                                                                    
  315  kubectl get quota                                                                                                                                                                              
  316  kubectl get quota -n myspace                                                                                                                                                                   
  317  kubectl delete -f helloworld-with-quota.yaml                                                                                                                                                   
  318  kubectl apply -f helloworld-with-quota.yaml                                                                                                                                                    
  319  kubectl get deploys -n myspace                                                                                                                                                                 
  320  kubectl get deploy -n myspace                                                                                                                                                                  
  321  kubectl get quota -n myspace                                                                                                                                                                   
  322  ls                                                                                                                                                                                             
  323  vim resourcequota.yaml                                                                                                                                                                         
  324  kubectl apply -f resourcequota.yaml                                                                                                                                                            
  325  kubectl get quota                                                                                                                                                                              
  326  kubectl get quota -n myspace                                                                                                                                                                   
  327  kubectl get deploys -n myspace                                                                                                                                                                 
  328  kubectl get deploy -n myspace                                                                                                                                                                  
  329  kubectl apply -f helloworld-with-quota.yaml                                                                                                                                                    
  330  kubectl get deploy -n myspace                                                                                                                                                                  
  331  kubectl describe deploy helloworld-deployment -n myspace                                                                                                                                       
  332  kubectl get quota                                                                                                                                                                              
  333  kubectl get quota -n myspace                                                                                                                                                                   
  334  kubectl get deploys -n myspace                                                                                                                                                                 
  335  kubectl get deploy -n myspace                                                                                                                                                                  
  336  kubectl get quota -n myspace                                                                                                                                                                   
  337  kubectl delete -f helloworld-with-quota.yaml                                                                                                                                                   
  338  kubectl create -f helloworld-with-quota.yaml                                                                                                                                                   
  339  kubectl get rs -n myspace                                                                                                                                                                      
  340  kubectl describe rs helloworld-deployment-9b4dccdd9 -n myspace                                                                                                                                 
  341  git status                                                                                                                                                                                     
  342  git pull                                                                                                                                                                                       
  343  kubectl delete -f .                                                                                                                                                                            
  344  kubectl get pods                                                                                                                                                                               
  345  cd ../16-User-Management/                                                                                                                                                                      
  346  ls                                                                                                                                                                                             
  347  cat REDAME.md                                                                                                                                                                                  
  348  openssl                                                                                                                                                                                        
  349  clear                                                                                                                                                                                          
  350  cat REDAME.md                                                                                                                                                                                  
  351  openssl genrsa -out jay.pem 2048                                                                                                                                                               
  352  ls                                                                                                                                                                                             
  353  mv jay.pem ~/                                                                                                                                                                                  
  354  cd ~/                                                                                                                                                                                          
  355  ls                                                                                                                                                                                             
  356  openssl  req -new -key jay.pem -out jay-csr.pem -subj "/CN=jay/O=training"                                                                                                                     
  357  ls                                                                                                                                                                                             
  358  cat jay-csr.pem                                                                                                                                                                                
  359  clear                                                                                                                                                                                          
  360  cd k8s-paypal-28-Dec-2020/16-User-Management/REDAME.md                                                                                                                                         
  361  cat k8s-paypal-28-Dec-2020/16-User-Management/REDAME.md                                                                                                                                        
  362  openssl x509 -req -in jay-csr.pem  -CA /etc/kubernetes/pki/ca.crt -CAkey /etc/kubernetes/pki/ca.key -CAcreateserial -out jay.crt 1000                                                          
  363  openssl x509 -req -in jay-csr.pem -CA /etc/kubernetes/pki/ca.crt -CAkey /etc/kubernetes/pki/ca.key -CAcreateserial -out jay.crt 1000                                                           
  364  openssl x509 -req -in jay-csr.pem -CA /etc/kubernetes/pki/ca.crt -CAkey /etc/kubernetes/pki/ca.key -CAcreateserial -out jay.crt -days 1000                                                     
  365  cat k8s-paypal-28-Dec-2020/16-User-Management/REDAME.md                                                                                                                                        
  366  openssl x509 -in jay.crt --text --noout                                                                                                                                                        
  367  openssl x509 -in jay.crt -text -noout                                                                                                                                                          
  368  ls                                                                                                                                                                                             
  369  clear                                                                                                                                                                                          
  370  cat k8s-paypal-28-Dec-2020/16-User-Management/REDAME.md                                                                                                                                        
  371  kubectl config view                                                                                                                                                                            
  372  kubectl config set-credentials -h                                                                                                                                                              
  373  kubectl config set-credentials jay --client-certificate=/root/jay.crt --client-key=/root/jay.pem                                                                                               
  374  kubectl config view                                                                                                                                                                            
  375  cat k8s-paypal-28-Dec-2020/16-User-Management/REDAME.md                                                                                                                                        
  376  kubectl config get-contexts                                                                                                                                                                    
  377  kubectl config set-context jay@kubernetes --cluster=kubernetes --user=jay                                                                                                                      
  378  kubectl config get-contexts                                                                                                                                                                    
  379  kubectl config use-context jay@kubernetes                                                                                                                                                      
  380  kubectl get pods                                                                                                                                                                               
  381  kubectl config use-context kubernetes-admin@kubernetes                                                                                                                                         
  382  kubectl get pods                                                                                                                                                                               
  383  cd k8s-paypal-28-Dec-2020/                                                                                                                                                                     
  384  git pull                                                                                                                                                                                       
  385  clear                                                                                                                                                                                          
  386  cd 17-RBAC/                                                                                                                                                                                    
  387  ls                                                                                                                                                                                             
  388  cat README.md                                                                                                                                                                                  
  389  kubectl create role deploy-reader --verb=get,list,watch --resource=deployments --dry-run -o yaml                                                                                               
  390  kubectl create role deploy-reader --verb=get,list,watch --resource=deployments --dry-run -o yaml > deploy-reader.yaml                                                                          
  391  kubectl create rolebinding deploy-reader-binding --role=deploy-reader --user=jay --dry-run -o yaml                                                                                             
  392  kubectl create rolebinding deploy-reader-binding --role=deploy-reader --user=jay --dry-run -o yaml > deploy-reader-binding.yaml                                                                
  393  ls                                                                                                                                                                                             
  394  kubectl apply -f deploy-reader.yaml                                                                                                                                                            
  395  kubectl apply -f deploy-reader-binding.yaml                                                                                                                                                    
  396  kubectl config get-context                                                                                                                                                                     
  397  kubectl config get-contexts                                                                                                                                                                    
  398  kubectl config use-context jay@kubernetes                                                                                                                                                      
  399  kubectl config get-contexts                                                                                                                                                                    
  400  kubectl config set-context --help                                                                                                                                                              
  401  kubectl config set-config --current --namespace=myspace                                                                                                                                        
  402  kubectl config set-context --current --namespace=myspace                                                                                                                                       
  403  kubectl config get-contexts                                                                                                                                                                    
  404  kubectl get pods                                                                                                                                                                               
  405  kubectl get deploys                                                                                                                                                                            
  406  kubectl get deploy                                                                                                                                                                             
  407  kubectl get deploy -n default                                                                                                                                                                  
  408  kubectl get pods -n default                                                                                                                                                                    
  409  kubectl config get-contexts                                                                                                                                                                    
  410  ls                                                                                                                                                                                             
  411  kubectl apply -f pod-reader-role.yaml                                                                                                                                                          
  412  kubectl config get-contexts                                                                                                                                                                    
  413  kubectl config use-context kubernetes-admin@kubernetes                                                                                                                                         
  414  kubectl get roles                                                                                                                                                                              
  415  kubectl describe roles deploy-reader                                                                                                                                                           
  416  kubectl describe rolebinding deploy-reader-binding                                                                                                                                             
  417  ls                                                                                                                                                                                             
  418  kubectl apply -f pod-reader-role.yaml read-pod-binding.yaml                                                                                                                                    
  419  kubectl apply -f pod-reader-role.yaml,read-pod-binding.yaml                                                                                                                                    
  420  kubectl describe role pod-reader-role                                                                                                                                                          
  421  kubectl get roles                                                                                                                                                                              
  422  kubectl describe role pod-reader                                                                                                                                                               
  423  vim pod-reader-role.yaml                                                                                                                                                                       
  424  cd ../                                                                                                                                                                                         
  425  git pull                                                                                                                                                                                       
  426  cd 17-RBAC/                                                                                                                                                                                    
  427  ls                                                                                                                                                                                             
  428  vun README.md                                                                                                                                                                                  
  429  vim README.md                                                                                                                                                                                  
  430  kubectl get clusterroles                                                                                                                                                                       
  431  kubectl describe clusterrole cluster-admin                                                                                                                                                     
  432  kubectl describe clusterrolebinding cluster-admin                                                                                                                                              
  433  kubectl create clusterrolebinding admin-user-jay --cluster=kubernetes --role=cluster-admin --user=jay                                                                                          
  434  kubectl create clusterrolebinding admin-user-jay --cluster=kubernetes --clusterrole=cluster-admin --user=jay                                                                                   
  435  vim README.md                                                                                                                                                                                  
  436  kubectl get clusterrolebindings admin-user-jay                                                                                                                                                 
  437  kubectl config get-contexts                                                                                                                                                                    
  438  kubectl config use-context jay@kubernetes                                                                                                                                                      
  439  kubectl get pods -A                                                                                                                                                                            
  440  kubectl get pods                                                                                                                                                                               
  441  kubectl config get-context                                                                                                                                                                     
  442  kubectl config get-contexts                                                                                                                                                                    
  443  kubectl config use-context kubernetes-admin@kubernetes                                                                                                                                         
  444  git pull                                                                                                                                                                                       
  445  cd ../18-Statefulset/                                                                                                                                                                          
  446  ls                                                                                                                                                                                             
  447  vim History                                                                                                                                                                                    
  448  kubectl get statefulset                                                                                                                                                                        
  449  git pull                                                                                                                                                                                       
  450  ls                                                                                                                                                                                             
  451  cat helloworld.yaml                                                                                                                                                                            
  452  kubectl create -f helloworld.yaml                                                                                                                                                              
  453  kubectl get statefulset                                                                                                                                                                        
  454  kubectl get pods -w                                                                                                                                                                            
  455  clear                                                                                                                                                                                          
  456  kubectl get pods                                                                                                                                                                               
  457  kubectl scale --replica=10 statefulset helloworld-statefull                                                                                                                                    
  458  vim History                                                                                                                                                                                    
  459  kubectl scale --replicas=10 statefulset helloworld-statefull                                                                                                                                   
  460  kubectl get pods -w                                                                                                                                                                            
  461  kubectl describe pods helloworld-statefull-0                                                                                                                                                   
  462  kubectl set image k8s-demo=amitvashist7/k8s-tiny-web:2 statefulset helloworld-statefull                                                                                                        
  463  vim History                                                                                                                                                                                    
  464  kubectl set image k8s-demo=amitvashist7/k8s-tiny-web:2 statefulset helloworld-statefull --record                                                                                               
  465  kubectl get statefulset                                                                                                                                                                        
  466  kubectl set image k8s-demo=amitvashist7/k8s-tiny-web:2 statefulset helloworld-statefull --record                                                                                               
  467  vim History                                                                                                                                                                                    
  468  kubectl set image statefulset/helloworld-statefull k8s-demo=amitvashist7/k8s-tiny-web:2 --record                                                                                               
  469  vim History                                                                                                                                                                                    
  470  kubectl get pods -w                                                                                                                                                                            
  471  ls                                                                                                                                                                                             
  472  vim History                                                                                                                                                                                    
  473  git pull                                                                                                                                                                                       
  474  kubectl delete -f helloworld.yaml                                                                                                                                                              
  475  cd ../19-DaemonSet/                                                                                                                                                                            
  476  ls                                                                                                                                                                                             
  477  cat History                                                                                                                                                                                    
  478  cat helloworld.yaml                                                                                                                                                                            
  479  kubectl create -f helloworld.yaml                                                                                                                                                              
  480  kubectl get ds                                                                                                                                                                                 
  481  kubectl get ds -o wide                                                                                                                                                                         
  482  kubectl get pods -o wide                                                                                                                                                                       
  483  cd /etc/kubernetes/manifests/                                                                                                                                                                  
  484  ls                                                                                                                                                                                             
  485  cat kube-apiserver.yaml                                                                                                                                                                        
  486  cat kube-apiserver.yaml  | grep -i toler                                                                                                                                                       
  487  ls                                                                                                                                                                                             
  488  cat etcd.yaml                                                                                                                                                                                  
  489  ls                                                                                                                                                                                             
  490  cat kube-scheduler.yaml                                                                                                                                                                        
  491  ls                                                                                                                                                                                             
  492  cat kube-controller-manager.yaml                                                                                                                                                               
  493  kubectl get ds -n kube-system                                                                                                                                                                  
  494  kubectl descrive ds kube-proxy                                                                                                                                                                 
  495  kubectl describe ds kube-proxy                                                                                                                                                                 
  496  kubectl describe ds kube-proxy -n kube-system                                                                                                                                                  
  497  kubectl get ds kube-proxy -n kube-system -o yaml                                                                                                                                               
  498  kubectl get nodes -o wide                                                                                                                                                                      
  499  kubectl get nodes --help                                                                                                                                                                       
  500  kubectl get nodes                                                                                                                                                                              
  501  kubectl descrive nodes kube-master                                                                                                                                                             
  502  kubectl describe nodes kube-master                                                                                                                                                             
  503  kubectl get nodes kube-master -o yaml                                                                                                                                                          
  504  clear                                                                                                                                                                                          
  505  cd -                                                                                                                                                                                           
  506  git pull                                                                                                                                                                                       
  507  kubectl delete -f .                                                                                                                                                                            
  508  cd ../20-Taint-and-Toleration/                                                                                                                                                                 
  509  ls                                                                                                                                                                                             
  510  vim README.md                                                                                                                                                                                  
  511  kubectl get pods                                                                                                                                                                               
  512  cat README.md                                                                                                                                                                                  
  513  kubectl taint nodes worker02 app=myapp:NoSchedule                                                                                                                                              
  514  kubectl get nodes worker02 -0 json                                                                                                                                                             
  515  kubectl get nodes worker02 -o json                                                                                                                                                             
  516  kubectl get nodes worker02 -o json | jq .spec.taints                                                                                                                                           
  517  apt-get install jq                                                                                                                                                                             
  518  kubectl get nodes worker02 -o json | jq .spec.taints                                                                                                                                           
  519  vim helloworld                                                                                                                                                                                 
  520  vim helloworld.yaml                                                                                                                                                                            
  521  kubectl create -f helloworld.yaml                                                                                                                                                              
  522  kubectl get deploy                                                                                                                                                                             
  523  kubectl get pods -w                                                                                                                                                                            
  524  kubectl get pods o wide                                                                                                                                                                        
  525  kubectl get pods -o wide                                                                                                                                                                       
  526  kubectl delete -f helloworld.yaml                                                                                                                                                              
  527  vim helloworld.yaml                                                                                                                                                                            
  528  kubectl create -f helloworld.yaml                                                                                                                                                              
  529  kubectl get pods -o wide                                                                                                                                                                       
  530  kubectl delete -f helloworld.yaml                                                                                                                                                              
  531  vim helloworld                                                                                                                                                                                 
  532  vim helloworld.yaml                                                                                                                                                                            
  533  kubectl get pods -o wide                                                                                                                                                                       
  534  kubectl create -f helloworld.yaml                                                                                                                                                              
  535  kubectl get pods -o wide                                                                                                                                                                       
  536  kubectl get nodes worker02 -o json | jq .spec.taints                                                                                                                                           
  537  kubectl get nodes worker01 -o json | jq .spec.taints                                                                                                                                           
  538  kubectl delete -f helloworld.yaml                                                                                                                                                              
  539  vim helloworld.yaml                                                                                                                                                                            
  540  kubectl create -f helloworld.yaml                                                                                                                                                              
  541  kubectl get pods -o wide                                                                                                                                                                       
  542  kubectl taint nodes worker01 test=test:NoExecute                                                                                                                                               
  543  kubectl get pods -o wide                                                                                                                                                                       
  544  kubectl get nodes worker01 -o json | jq .spec.taints                                                                                                                                           
  545  kubectl get nodes worker02 -o json | jq .spec.taints                                                                                                                                           
  546  kubectl delete -f helloworld.yaml                                                                                                                                                              
  547  vim helloworld.yaml                                                                                                                                                                            
  548  kubectl create -f helloworld.yaml                                                                                                                                                              
  549  kubectl get pods -o wide                                                                                                                                                                       
  550  ls                                                                                                                                                                                             
  551  cat README.md                                                                                                                                                                                  
  552  kubectl taint node worker01 test-                                                                                                                                                              
  553  kubectl taint node worker02 app-                                                                                                                                                               
  554  clear                                                                                                                                                                                          
  555  kubectl delete -f .                                                                                                                                                                            
  556  cd ../                                                                                                                                                                                         
  557  clear                                                                                                                                                                                          
  558  git pull                                                                                                                                                                                       
  559  cd 21-Affinity/                                                                                                                                                                                
  560  ls                                                                                                                                                                                             
  561  cat helloworld                                                                                                                                                                                 
  562  cat helloworld.yaml                                                                                                                                                                            
  563  cat helloworld-dev-prod.yaml                                                                                                                                                                   
  564  cat helloworld-multi-affinity.yaml                                                                                                                                                             
  565  ls                                                                                                                                                                                             
  566  kubectl create -f helloworld.yaml                                                                                                                                                              
  567  kubectl get deploys                                                                                                                                                                            
  568  kubectl get deploy                                                                                                                                                                             
  569  kubectl get pods                                                                                                                                                                               
  570  vim helloworld                                                                                                                                                                                 
  571  vim helloworld.yaml                                                                                                                                                                            
  572  kubectl get nodes --show-label                                                                                                                                                                 
  573  kubectl get nodes --show-labels                                                                                                                                                                
  574  kubectl label node worker02 env-                                                                                                                                                               
  575  kubectl get nodes --show-label                                                                                                                                                                 
  576  kubectl get nodes --show-labels                                                                                                                                                                
  577  kubectl delete -f helloworld                                                                                                                                                                   
  578  kubectl delete -f helloworld.yaml                                                                                                                                                              
  579  kubectl get pods                                                                                                                                                                               
  580  kubectl create -f helloworld.yaml                                                                                                                                                              
  581  kubectl get pods                                                                                                                                                                               
  582  kubectl get rs                                                                                                                                                                                 
  583  kubectl describe rs helloworld-deployment-b64578fb                                                                                                                                             
  584  kubectl describe pods helloworld-deployment-b64578fb-t7xrc                                                                                                                                     
  585  kubectl label nodes worker01 env=prod                                                                                                                                                          
  586  kubectl get deploy                                                                                                                                                                             
  587  kubectl get rs                                                                                                                                                                                 
  588  kubectl get pods                                                                                                                                                                               
  589  kubectl get pods -o wide                                                                                                                                                                       
  590  kubectl label nodes worker01 env-                                                                                                                                                              
  591  kubectl get pods -o wide                                                                                                                                                                       
  592  kubectl scale --replicas=5 deploy helloworld-deployment                                                                                                                                        
  593  kubectl get pods -o wide                                                                                                                                                                       
  594  kubectl label nodes worker02 env=dev                                                                                                                                                           
  595  kubectl get pods -o wide                                                                                                                                                                       
  596  kubectl label nodes worker02 env=prod                                                                                                                                                          
  597  kubectl label nodes worker02 env=prod --overrite                                                                                                                                               
  598  kubectl label nodes worker02 env=prod --overwrite                                                                                                                                              
  599  kubectl get pods                                                                                                                                                                               
  600  kubectl get pods -o wide                                                                                                                                                                       
  601  ls                                                                                                                                                                                             
  602  vim helloworld-dev-prod.yaml                                                                                                                                                                   
  603  kubectl delete -f helloworld.yaml                                                                                                                                                              
  604  kubectl get pods                                                                                                                                                                               
  605  kubectl get nodes --show-labels                                                                                                                                                                
  606  kubectl label node worker01 env=dev                                                                                                                                                            
  607  ls                                                                                                                                                                                             
  608  kubectl apply -f helloworld-dev-prod.yaml                                                                                                                                                      
  609  kubectl get pods                                                                                                                                                                               
  610  kubectl get pods -o wide                                                                                                                                                                       
  611  kubectl label nodes worker01 env-                                                                                                                                                              
  612  kubectl get pods -o wide                                                                                                                                                                       
  613  kubectl label node worker01 env=deb                                                                                                                                                            
  614  kubectl label node worker01 env=dev --overwrite                                                                                                                                                
  615  kubectl get pods                                                                                                                                                                               
  616  kubectl delete -f helloworld-dev-prod.yaml                                                                                                                                                     
  617  ls                                                                                                                                                                                             
  618  vim helloworld-multi-affinity.yaml                                                                                                                                                             
  619  cat helloworld-multi-affinity.yaml                                                                                                                                                             
  620  ls                                                                                                                                                                                             
  621  kubectl create -f helloworld-multi-affinity.yaml                                                                                                                                               
  622  kubectl get pods                                                                                                                                                                               
  623  kubectl get nodes --show-labels                                                                                                                                                                
  624  ls                                                                                                                                                                                             
  625  vim helloworld-multi-affinity.yaml                                                                                                                                                             
  626  kubectl get pods -o wide                                                                                                                                                                       
  627  kubectl label node worker02 env-dev --override                                                                                                                                                 
  628  kubectl label node worker02 env-dev --overwrite                                                                                                                                                
  629  kubectl get pods                                                                                                                                                                               
  630  ls                                                                                                                                                                                             
  631  kubectl delete -f helloworld-multi-affinity.yaml                                                                                                                                               
  632  kubectl get pods                                                                                                                                                                               
  633  kubectl label node worker01 team=test                                                                                                                                                          
  634  kubectl apply -f helloworld-multi-affinity.yaml                                                                                                                                                
  635  kubectl get pods                                                                                                                                                                               
  636  kubectl get pods -o wide                                                                                                                                                                       
  637  kubectl get nodes --show-labels                                                                                                                                                                
  638  kubectl label nodes worker02 env=dev --overwrite                                                                                                                                               
  639  kubectl get nodes --show-labels                                                                                                                                                                
  640  kubectl delete -f helloworld-multi-affinity.yaml                                                                                                                                               
  641  kubectl get pods                                                                                                                                                                               
  642  kubectl apply -f helloworld-multi-affinity.yaml                                                                                                                                                
  643  kubectl get pods                                                                                                                                                                               
  644  kubectl get pods -o wide                                                                                                                                                                       
  645  git pull                                                                                                                                                                                       
  646  kubectl delete -f helloworld-multi-affinity.yaml                                                                                                                                               
  647  kubectl get nodes --show-labels                                                                                                                                                                
  648  kubectl label nodes worker01 env-,team-                                                                                                                                                        
  649  kubectl label nodes worker01 env- team-                                                                                                                                                        
  650  kubectl get nodes --show-labels                                                                                                                                                                
  651  kubectl label nodes worker02 env- hardware-                                                                                                                                                    
  652  kubectl get nodes --show-labels                                                                                                                                                                
  653  cd ../                                                                                                                                                                                         
  654  ls                                                                                                                                                                                             
  655  cd 22-Pod-Affinity-and-Anti-Affinity/                                                                                                                                                          
  656  ls                                                                                                                                                                                             
  657  kubectl apply -f helloworld.yaml                                                                                                                                                               
  658  kubectl get pods                                                                                                                                                                               
  659  kubectl get pods -o wide                                                                                                                                                                       
  660  kubectl get nodes kube-master -o json | jq .spec.taints                                                                                                                                        
  661  kubectl taint nodes kube-master node-role.kubernetes.io/master-                                                                                                                                
  662  kubectl get nodes                                                                                                                                                                              
  663  kubectl get pods -o wide                                                                                                                                                                       
  664  kubectl taint nodes kube-master node-role.kubernetes.io/master:NoSchedule                                                                                                                      
  665  kubectl get pods -o wide                                                                                                                                                                       
  666  kubectl delete -f helloworld.yaml                                                                                                                                                              
  667  kubectl get pods                                                                                                                                                                               
  668  git pull                                                                                                                                                                                       
  669  kubectl delete -f .                                                                                                                                                                            
  670  kubectl get deplots                                                                                                                                                                            
  671  kubectl get deploy                                                                                                                                                                             
  672  cd ../23-Taint-and-toleration-with-affinity/                                                                                                                                                   
  673  ls                                                                                                                                                                                             
  674  cat helloworld-affinity                                                                                                                                                                        
  675  cat helloworld-affinity.yaml                                                                                                                                                                   
  676  ls                                                                                                                                                                                             
  677  cat helloworld-affinity.yaml                                                                                                                                                                   
  678  kubectl get node --show-labels                                                                                                                                                                 
  679  ls                                                                                                                                                                                             
  680  kubectl apply -f helloworld-affinity.yaml                                                                                                                                                      
  681  kubectl get deploys                                                                                                                                                                            
  682  kubectl get deploy                                                                                                                                                                             
  683  kubectl get pods                                                                                                                                                                               
  684  cat helloworld-affinity.yaml                                                                                                                                                                   
  685  kubectl label node kube-master team=engineering-project1                                                                                                                                       
  686  kubectl label node worker01 team=engineering-project1                                                                                                                                          
  687  kubectl get pods                                                                                                                                                                               
  688  kubectl get pods -o wide                                                                                                                                                                       
  689  kubectl taint nodes kube-master node-role.kubernetes.io/master-                                                                                                                                
  690  ls                                                                                                                                                                                             
  691  kubectl delete -f helloworld-affinity.yaml                                                                                                                                                     
  692  kubectl create -f helloworld-affinity.yaml                                                                                                                                                     
  693  kubect get pods -o wide                                                                                                                                                                        
  694  kubectl get pods -o wide                                                                                                                                                                       
  695  ls                                                                                                                                                                                             
  696  vim helloworld-affinity-with-tolerations.yaml                                                                                                                                                  
  697  kubectl taint nodes worker02 app=myapp:NoSchedule                                                                                                                                              
  698  ls                                                                                                                                                                                             
  699  kubectl create -f helloworld-affinity-with-tolerations.yaml                                                                                                                                    
  700  kubectl get pods -o wide                                                                                                                                                                       
  701  lss                                                                                                                                                                                            
  702  ls                                                                                                                                                                                             
  703  vim helloworld-affinity-with-tolerations.yaml                                                                                                                                                  
  704  kubectl get nodes --show-labels                                                                                                                                                                
  705  kubectl get pods -o wide                                                                                                                                                                       
  706  clear                                                                                                                                                                                          
  707  kubectl get pods                                                                                                                                                                               
  708  kubectl delete deploys helloworld-deployment                                                                                                                                                   
  709  kubectl delete deploy helloworld-deployment                                                                                                                                                    
  710  kubectl get pods                                                                                                                                                                               
  711  git pull                                                                                                                                                                                       
  712  cd ..                                                                                                                                                                                          
  713  cd 26-Volumes-NFS/                                                                                                                                                                             
  714  ls                                                                                                                                                                                             
  715  clear                                                                                                                                                                                          
  716  ls                                                                                                                                                                                             
  717  vim README.md                                                                                                                                                                                  
  718  apt-get install nfs-kernel-server -y                                                                                                                                                           
  719  cat README.md                                                                                                                                                                                  
  720  mkdir /exports                                                                                                                                                                                 
  721  chown nobody:nogroup /exports                                                                                                                                                                  
  722  grep -i exports /etc/exports                                                                                                                                                                   
  723  vim /etc/exports                                                                                                                                                                               
  724  systemctl restart nfs-kernel-server                                                                                                                                                            
  725  systemctl status nfs-kernel-server                                                                                                                                                             
  726  showmount -e localhost                                                                                                                                                                         
  727  systemctl status nfs-kernel-server                                                                                                                                                             
  728  ls                                                                                                                                                                                             
  729  cat pv-nfs.yaml                                                                                                                                                                                
  730  kubectl get pv                                                                                                                                                                                 
  731  kubectl create -f pv-nfs.yaml                                                                                                                                                                  
  732  kubectl get pv                                                                                                                                                                                 
  733  clear                                                                                                                                                                                          
  734  ls                                                                                                                                                                                             
  735  kubectl get pv                                                                                                                                                                                 
  736  cat pv-nfs.yaml                                                                                                                                                                                
  737  cat pvc-nfs.yaml                                                                                                                                                                               
  738  kubectl get pvc                                                                                                                                                                                
  739  kubectl create -f pvc-nfs.yaml                                                                                                                                                                 
  740  kubectl get pvc                                                                                                                                                                                
  741  kubectl get pv                                                                                                                                                                                 
  742  ls                                                                                                                                                                                             
  743  cat nfs-busybox-rc.yaml                                                                                                                                                                        
  744  cat web-rc-pvc.yaml                                                                                                                                                                            
  745  clear                                                                                                                                                                                          
  746  ls                                                                                                                                                                                             
  747  cat nfs-busybox-rc.yaml                                                                                                                                                                        
  748  kubectl get pods                                                                                                                                                                               
  749  kubectl delete deploy helloworld-deployment-at                                                                                                                                                 
  750  kubectl delete deploy wordpress-deployment                                                                                                                                                     
  751  kubectl create -f nfs-busybox-rc.yaml                                                                                                                                                          
  752  kubectl get pods                                                                                                                                                                               
  753  cat /exports/index.html                                                                                                                                                                        
  754  clear                                                                                                                                                                                          
  755  ls                                                                                                                                                                                             
  756  cat nfs-web-svc.yaml                                                                                                                                                                           
  757  cat web-rc-pvc.yaml                                                                                                                                                                            
  758  kubectl create -f web-rc-pvc.yaml                                                                                                                                                              
  759  kubectl get rc                                                                                                                                                                                 
  760  ls                                                                                                                                                                                             
  761  cat nfs-web-svc.yaml                                                                                                                                                                           
  762  kubectl create -f nfs-web-svc.yaml                                                                                                                                                             
  763  kubectl get svc                                                                                                                                                                                
  764  kubectl delete svc wordpress-service                                                                                                                                                           
  765  kubectl edit svc nfs-web-svc.yaml                                                                                                                                                              
  766  kubectl edit svc nfs-web-                                                                                                                                                                      
  767  kubectl edit svc nfs-web                                                                                                                                                                       
  768  kubectl get svc                                                                                                                                                                                
  769  > /exports/index.html                                                                                                                                                                          
  770  kubectl get pods                                                                                                                                                                               
  771  kubectl delete pods nfs-busybox-2-5rsrx nfs-busybox-2-gf59n nfs-busybox-2-mkbgg                                                                                                                
  772  kubectl get pods                                                                                                                                                                               
  773  history                                                                                                                                                                                        
  774  git pull                                                                                                                                                                                       
  775  cd ../                                                                                                                                                                                         
  776  ls                                                                                                                                                                                             
  777  cd 27-AutoScaling/                                                                                                                                                                             
  778  ls                                                                                                                                                                                             
  779  cat hpa-example-deploy.yaml                                                                                                                                                                    
  780  while true; do curl http://35.184.38.244:31001; done;                                                                                                                                          
  781  apt-get install helm                                                                                                                                                                           
  782  apt-list madison helm                                                                                                                                                                          
  783  apt-search madison helm                                                                                                                                                                        
  784  apt-cache madison helm                                                                                                                                                                         
  785  apt-cache list heml                                                                                                                                                                            
  786  apt-cache --help                                                                                                                                                                               
  787  apt-cache search hlm                                                                                                                                                                           
  788  apt-cache search helm                                                                                                                                                                          
  789  curl https://baltocdn.com/helm/signing.asc | sudo apt-key add -                                                                                                                                
  790  sudo apt-get install apt-transport-https --yes                                                                                                                                                 
  791  echo "deb https://baltocdn.com/helm/stable/debian/ all main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list                                                                        
  792  sudo apt-get update                                                                                                                                                                            
  793  sudo apt-get install helm                                                                                                                                                                      
  794  kubectl get pods                                                                                                                                                                               
  795  kubectl delete -f .                                                                                                                                                                            
  796  ls                                                                                                                                                                                             
  797  sudo apt-get install helm                                                                                                                                                                      
  798  helm -v                                                                                                                                                                                        
  799  helm version                                                                                                                                                                                   
  800  clear                                                                                                                                                                                          
  801  git pull                                                                                                                                                                                       
  802  cd ../                                                                                                                                                                                         
  803  ls                                                                                                                                                                                             
  804  cd 29-Helm/                                                                                                                                                                                    
  805  ls                                                                                                                                                                                             
  806  cat README.md                                                                                                                                                                                  
  807  kubectl create -f helm-rbac.yaml                                                                                                                                                               
  808  helm init --service-account tiller --override spec.selector.matchLabels.'name'='tiller',spec.selector.matchLabels.'app'='helm' --output yaml | sed 's@apiVersion: extensions/v1beta1@apiVersion
' | kubectl apply -f -                                                                                                                                                                                
  809  helm --help                                                                                                                                                                                    
  810  ls                                                                                                                                                                                             
  811  cat README.md                                                                                                                                                                                  
  812  helm version                                                                                                                                                                                   
  813  clear                                                                                                                                                                                          
  814  cat README.md                                                                                                                                                                                  
  815  helm init                                                                                                                                                                                      
  816  helm repo add azure-marketplace https://marketplace.azurecr.io/helm/v1/repo                                                                                                                    
  817  kubectl get pods                                                                                                                                                                               
  818  helm init                                                                                                                                                                                      
  819  helm version                                                                                                                                                                                   
  820  ls                                                                                                                                                                                             
  821  cat README.md                                                                                                                                                                                  
  822  helm repo add azure-marketplace https://marketplace.azurecr.io/helm/v1/repo                                                                                                                    
  823  helm search wordpress                                                                                                                                                                          
  824  cd ../                                                                                                                                                                                         
  825  ls                                                                                                                                                                                             
  826  cd ../                                                                                                                                                                                         
  827  ls                                                                                                                                                                                             
  828  cd k8s                                                                                                                                                                                         
  829  ls                                                                                                                                                                                             
  830  history > HISTORY.txt                                                                                                                                                                          
root@kube-master:~/k8s#                                                                                                                                                                               
