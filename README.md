# k8s-wordpress


## create cluster prod
```sh
gcloud container clusters create production  --labels=environment=production,v=1,operator=mesaquesilva --min-nodes=2 --max-nodes=13 --enable-autoscaling --node-labels=environment=production
```

## create cluster test
```sh 
gcloud container clusters create development  --labels=environment=development,v=1,operator=mesaquesilva --num-nodes=1 --node-labels=environment=development
```