 ES HIGH AVAILABLE CLUSTER
 
 - Cluster runs on 3 dedicated nodes of a kubernetes cluster where nodes are tainted with elasticsearch labels , which es-cluster StatefulSet pods have tolerations.
 - Prod requirement for resources (cpu,memory and storage requirements of the pods)  are ignored in this demo.
 - Elasticsearch Beat  configurations ( as DaemonSets ) are not included and can be discussed separetely.
