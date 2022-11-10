# Commands

## Git

`code` `git add .` `git commit -m "message"` `git push`

## Docker

`code` `docker build -t image_name .` `docker run -p 8080:8080 image_name`

## Docker Compose

`code` `docker-compose up` `docker-compose up -d` `docker-compose down`

## Docker Swarm

`code` `docker swarm init` `docker stack deploy -c docker-compose.yml stack_name` `docker stack rm stack_name`

## Kubernetes

`code` `kubectl apply -f k8s` `kubectl delete -f k8s`

## Helm

`code` `helm install --name release_name chart_name` `helm delete --purge release_name`

## AWS

`code` `aws configure` `aws s3 ls` `aws s3 mb s3://bucket_name` `aws s3 cp file_name s3://bucket_name` `aws s3 rm s3://bucket_name/file_name` `aws s3 rb s3://bucket_name`

## AWS Elastic Beanstalk

`code` `eb init` `eb create` `eb deploy` `eb open` `eb status` `eb logs` `eb terminate`

## AWS Elastic Container Service

`code` `ecs-cli configure --cluster cluster_name --default-launch-type EC2 --config-name cluster_name --region region` `ecs-cli up --keypair keypair_name --capability-iam --size 1 --instance-type t2.micro` `ecs-cli compose --file docker-compose.yml service up` `ecs-cli compose --file docker-compose.yml service down` `ecs-cli down --force`

## AWS Elastic Kubernetes Service

`code` `aws eks --region region update-kubeconfig --name cluster_name` `kubectl apply -f k8s` `kubectl delete -f k8s`

## AWS Elastic Container Registry

`code` `aws ecr get-login --no-include-email --region region` `docker build -t image_name .` `docker tag image_name:latest account_id.dkr.ecr.region.amazonaws.com/image_name:latest` `docker push account_id.dkr.ecr.region.amazonaws.com/image_name:latest`

## AWS Lambda

`code` `aws lambda create-function --function-name function_name --runtime nodejs8.10 --role role_arn --handler index.handler --zip-file fileb://function.zip` `aws lambda update-function-code --function-name function_name --zip-file fileb://function.zip` `aws lambda invoke --function-name function_name output.txt` `aws lambda delete-function --function-name function_name`
