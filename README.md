#################################
#
#  Instructions
#

1. spun up EC2 instance in aws & installed minikube,docker,helm
2. started up minikube & enabled ingress addon
3. created helm charts with below structure:
igstest
├── Chart.yaml
├── README.md
├── charts
│   ├── frontend
│   │   ├── Chart.yaml
│   │   ├── templates
│   │   │   ├── deployment.yaml
│   │   │   ├── ingress.yaml
│   │   │   └── service.yaml
│   │   └── value.yaml
│   ├── service1
│   │   ├── Chart.yaml
│   │   ├── templates
│   │   │   ├── deployment.yaml
│   │   │   └── service.yaml
│   │   └── value.yaml
│   ├── service2
│   │   ├── Chart.yaml
│   │   ├── templates
│   │   │   ├── deployment.yaml
│   │   │   └── service.yaml
│   │   └── value.yaml
│   └── service3
│       ├── Chart.yaml
│       ├── templates
│       │   ├── deployment.yaml
│       │   └── service.yaml
│       └── value.yaml
├── requirements.yaml
├── templates
└── values.yaml
10 directories, 21 files

4. I have uploaded all these file in repo:  https://github.com/edjwhho/igstest
5. To run, just clone the repo ie. git clone https://github.com/edjwhho/igstest
6. cd igstest
7. All the charts for frontend / service1 / service2 /service3 are located in igstest/charts
8. To run the charts just run this command:  helm install igstest .

Expected output:
NAME: igstest
LAST DEPLOYED: Tue Dec  3 21:17:50 2019
NAMESPACE: default
STATUS: deployed
REVISION: 1
TEST SUITE: None


 
