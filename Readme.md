


Image information for the kubernetes cluster are used based on the infromation

voting app: kodekloud/examplevotingapp_vote:v1
result app: kodekloud/examplevotingapp_result:v1
redis: redis
postgres: postgresql
worker: kodekloud/examplevotingapp_worker:v1

Steps:
1. Deploy PODs
2. Create Services (ClusterIP)
    1. redis (name should be redis in metadata for the worker to connect)
    2. db (name should be db in metadata for the worker to connect)
3. Create Services (NodePort)
    1. voting-app
    2. result-app

Load the results from the following URLs

For voting app: http://localhost:30050
For results app: http://localhost:30051

# votingapp
