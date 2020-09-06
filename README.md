 ES HIGH AVAILABLE CLUSTER
 
 - Cluster runs on 3 dedicated nodes of a kubernetes cluster where nodes are tainted with elasticsearch labels , which es-cluster StatefulSet pods have tolerations.
 - Prod requirement for resources (cpu,memory and storage requirements of the pods)  are ignored in this demo.
 - Elasticsearch Beat  configurations ( as DaemonSets ) are not included and can be discussed separetely.
 - This cluster is tested on a AWS Kubernetes cluster , which is set up with kops :
 
kops create cluster <<cluster name>>  --node-count 5 --node-size t2.medium --master-count 1 --master-size t2.micro --zones eu-central-1c --topology public --    networking kube-router  --state <s3 bucket>
