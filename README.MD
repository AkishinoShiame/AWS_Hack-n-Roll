# [WorkShop-1] AWS CDK + AWS CloudFormation
  
## AWS CDK  
  
```bash
~ $ tree
.
├── README.md
├── assets
│   ├── package-lock.json
│   └── package.json
├── bin
│   └── app.ts
├── cdk.json
├── jest.config.js
├── lib
│   ├── iWorkshopStackProps.ts
│   └── stacks
│       └── helloWorldStack.ts
├── package-lock.json
├── package.json
├── slides
│   ├── cloud-101.pdf
│   └── workshop.pdf
└── tsconfig.json
```

> CDK uses above structure to look inside the define of "stacks" and knows how to build the structures and apps.  
>  
> CDK define APPS in cdk.js, call inside bin/app.ts  
>  
>> Inside bin/app.ts, it define the enviorment variables.  
>>  
>> <Stack>.ts will be define inside lib/stacks/<name>.ts, tells what infra stacks should be create.  
  
## Git Clone Content(Sub Module)  
  
| Sub-Module Repositories | Description |  
| --- | --- |  
| Local-With-CloudFormation @ f16d82d | [WorkShop-1 Related] Instructure Provides Easy Examples of CDK-with-onCloud-CloudFormation |  
| aws-cdk @ af56996 | [WorkShop-1 Related] AWS **C**loud **D**evelopment **K**it - Still only fully support TypeScript, like shit. Check [Prove](https://docs.aws.amazon.com/cdk/latest/guide/multiple_languages.html#multiple_languages) |  
| aws-cli @ 5596ec2 | [WorkShop-1 Related] AWS Command line tools |  
| aws-shell @ 8950f03 | [WorkShop-1 Related] AWS Shell bash tools |  
| troposphere @ 7f2aedd | [WorkShop-1 Related] A useful tool that a Python library to create AWS CloudFormation descriptions |  
  
## CDK Template  
  
**Clone Template to "Template" Folder**  
  
> https://docs.aws.amazon.com/ja_jp/cdk/latest/guide/about_examples.html  
>> https://docs.aws.amazon.com/en_pv/cdk/latest/guide/about_examples.html  
  
*Special* **CDK Python API** : https://docs.aws.amazon.com/cdk/api/latest/python/index.html  
  
Explane Coding languages supports status: 
  
> https://docs.aws.amazon.com/cdk/latest/guide/multiple_languages.html  
>> https://docs.aws.amazon.com/cdk/latest/guide/reference.html#aws_construct_lib_versioning_binding
  
**AWS Tools** : https://aws.amazon.com/jp/tools/  
  
Chapter of "Use an Existing AWS CloudFormation Template" *(Currently Suggest!!)* : https://docs.aws.amazon.com/cdk/latest/guide/use_cfn_template.html  
  
## AWS CDK Examples

The one listed belows inside "Template/" is [CDK Examples](https://github.com/aws-samples/aws-cdk-examples) cloned repo from GitHub includes the following examples\.
  
> Template/java  
> Template/python  
> Template/typescript  
>> Template/java/*  
>> Template/python/*  
>> Template/typescript/*  
  
### TypeScript examples<a name="typescript-examples"></a>


| Example | Description | 
| --- |--- |
| [api\-cors\-lambda\-crud\-dynamodb](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/api-cors-lambda-crud-dynamodb/) | Creating a single API with CORS, and five Lambdas doing CRUD operations over a single DynamoDB | 
| [application\-load\-balancer](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/application-load-balancer/) | Using an AutoScalingGroup with an Application Load Balancer | 
| [appsync\-graphql\-dynamodb](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/appsync-graphql-dynamodb/) | Creating a single GraphQL API with an API Key, and four Resolvers doing CRUD operations over a single DynamoDB | 
| [classic\-load\-balancer](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/classic-load-balancer/) | Using an AutoScalingGroup with a Classic Load Balancer | 
| [custom\-resource](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/custom-resource/) | Shows adding a Custom Resource to your CDK app | 
| [elasticbeanstalk](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/elasticbeanstalk/) | Elastic Beanstalk example using CFN resources with a Blue/Green pipeline \(community contributed\) | 
| [ecs\-cluster](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/ecs/cluster/) | Provision an ECS Cluster with custom Autoscaling Group configuration | 
| [ecs\-load\-balanced\-service](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/ecs/ecs-load-balanced-service/) | Starting a container fronted by a load balancer on ECS | 
| [ecs\-service\-with\-task\-placement](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/ecs/ecs-service-with-task-placement/) | Starting a container ECS with task placement specifications | 
| [ecs\-service\-with\-advanced\-alb\-config](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/ecs/ecs-service-with-advanced-alb-config/) | Starting a container fronted by a load balancer on ECS with added load balancer configuration | 
| [ecs\-service\-with\-task\-networking](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/ecs/ecs-service-with-task-networking/) | Starting an ECS service with task networking, allowing ingress traffic to the task but blocking for the instance | 
| [fargate\-load\-balanced\-service](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/ecs/fargate-load-balanced-service/) | Starting a container fronted by a load balancer on Fargate | 
| [fargate\-service\-with\-auto\-scaling](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/ecs/fargate-service-with-auto-scaling/) | Starting an ECS service of FARGATE launch type that auto scales based on average CPU Utilization | 
| [lambda\-cron](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/lambda-cron/) | Running a Lambda on a schedule | 
| [my\-widget\-service](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/my-widget-service/) | Use Lambda to serve up widgets | 
| [resource\-overrides](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/resource-overrides/) | Shows how to override generated CloudFormation code | 
| [static\-site](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/static-site/) | A static site using CloudFront | 
| [stepfunctions\-job\-poller](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/stepfunctions-job-poller/) | A simple StepFunctions workflow | 
| [ecs\-service\-with\-logging](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/ecs/ecs-service-with-logging/) | Starting a container fronted by a load balancer on ECS | 
| [fargate\-service\-with\-logging](https://github.com/aws-samples/aws-cdk-examples/tree/master/typescript/ecs/fargate-service-with-logging/) | Starting a container fronted by a load balancer on Fargate | 

### Java examples<a name="java-examples"></a>


| Example | Description | 
| --- |--- |
| [hello\-world](https://github.com/aws-samples/aws-cdk-examples/tree/master/java/hello-world/) | A demo application that uses the CDK in Java | 
| [lambda\-cron](https://github.com/aws-samples/aws-cdk-examples/tree/master/java/lambda-cron/) | Running a Lambda on a schedule | 

### Python examples<a name="python-examples"></a>


| Example | Description | 
| --- |--- |
| [application\-load\-balancer](https://github.com/aws-samples/aws-cdk-examples/tree/master/python/application-load-balancer/) | Using an AutoScalingGroup with an Application Load Balancer | 
| [classic\-load\-balancer](https://github.com/aws-samples/aws-cdk-examples/tree/master/python/classic-load-balancer/) | Using an AutoScalingGroup with a Classic Load Balancer | 
| [custom\-resource](https://github.com/aws-samples/aws-cdk-examples/tree/master/python/custom-resource/) | Shows adding a Custom Resource to your CDK app | 
| [ecs\-cluster](https://github.com/aws-samples/aws-cdk-examples/tree/master/python/ecs/cluster/) | Provision an ECS Cluster with custom Autoscaling Group configuration | 
| [ecs\-load\-balanced\-service](https://github.com/aws-samples/aws-cdk-examples/tree/master/python/ecs/ecs-load-balanced-service/) | Starting a container fronted by a load balancer on ECS | 
| [ecs\-service\-with\-task\-placement](https://github.com/aws-samples/aws-cdk-examples/tree/master/python/ecs/ecs-service-with-task-placement/) | Starting a container ECS with task placement specifications | 
| [ecs\-service\-with\-advanced\-alb\-config](https://github.com/aws-samples/aws-cdk-examples/tree/master/python/ecs/ecs-service-with-advanced-alb-config/) | Starting a container fronted by a load balancer on ECS with added load balancer configuration | 
| [ecs\-service\-with\-task\-networking](https://github.com/aws-samples/aws-cdk-examples/tree/master/python/ecs/ecs-service-with-task-networking/) | Starting an ECS service with task networking, allowing ingress traffic to the task but blocking for the instance | 
| [fargate\-load\-balanced\-service](https://github.com/aws-samples/aws-cdk-examples/tree/master/python/ecs/fargate-load-balanced-service/) | Starting a container fronted by a load balancer on Fargate | 
| [fargate\-service\-with\-autoscaling](https://github.com/aws-samples/aws-cdk-examples/tree/master/python/ecs/fargate-service-with-autoscaling/) | Starting an ECS service of FARGATE launch type that auto scales based on average CPU Utilization | 
| [lambda\-cron](https://github.com/aws-samples/aws-cdk-examples/tree/master/python/lambda-cron/) | Running a Lambda on a schedule | 
| [stepfunctions](https://github.com/aws-samples/aws-cdk-examples/tree/master/python/stepfunctions/) | A simple StepFunctions workflow | 

### JavaScript examples<a name="javascript-examples"></a>


| Example | Description | 
| --- |--- |
| [aws\-cdk\-changelogs\-demo](https://github.com/aws-samples/aws-cdk-changelogs-demo) | A full serverless Node\.js application stack deployed using CDK\. It uses AWS Lambda, AWS Fargate, DynamoDB, Elasticache, S3, and CloudFront\. | 
  
  
  
## Installation & Setup steps  
  
#### Enviorment Needed  
* [Node.js ≥ 10.3.0](https://nodejs.org/download/release/latest-v10.x/)  
* [NPM](https://www.npmjs.com/)  
* [NVM](https://github.com/nvm-sh/nvm)  
* [Docker(Optional)](https://www.docker.com/products/docker-desktop)  
* [K8S(Extended)](https://kubernetes.io/)  
  
#### Installation  
* Install above requires packages  
* AWS CDK CLI Install  
Command: `$ npm i -g aws-cdk`  
* Setup CDK CLI Token as belows  
 * create [AWS Account](https://portal.aws.amazon.com/billing/signup).  
 * Goes to [AWS IAM](https://console.aws.amazon.com/iam/) page.  
 * Create IAM user with corrisponding rights(Admin) and download **.CSV of Token**  
* Type belows information and type corrisponding below informations.   
```bash
[TestEnviormentHost:~ testuser$ aws configure
AWS Access Key ID []: <Type-your-Access-Key-ID-here-TIHH>
AWS Secret Access Key[]: <Type-your-Secret-Access-here-qhMb>
Default region name []: ap-northeast-1
Default output format []: text
```
[Mark]: the region name can be found in [here](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.RegionsAndAvailabilityZones.html) please use the shortest location near you.
* Last part to build project:  
```bash
$ cd <to-your-project-location>
$ npm install typescript
$ << Edit your stack/codes/files >>
$ cdk bootstrap  # bootstrap from local to cloud.
$ cdk deploy <stack>  # assign a stack to deploy to AWS.
$ cdk destroy  # clean up if you want to destroy the deployment. *Note: storage must be empty!*
```
**Currently suggest building CDK with typescript code(If you knows), or using CloudFormation Template with CDK to build your project** (´っ･ω･)っ  
  
  
# [WorkShop-2] Domain Driven Design

| STRATEGY | TATICAL |   
| --- | --- |  
| The Concepts / Structure Create / Design | The actual method: EX; language select / actual doing |  
  
<h3>Respect the god (Experiencer) [Domain Knowledger]. </h3>  
  
#### Domain Gathering  
  
* Needs Different Domain Knowledger Join.  
* Communication is Importent.  
* Respect the GODs.  
* Try to check from other side (EX: UE/UI/UX).  
* Try to Learn and Speak with same language.  
  
#### Domain Gathering TOOL  
> Event Storming.
  
* Sliding Time-line to specific Event.  
* Brain Storming and Create Idea / Think more wider.  
* Create concept from currently exist.  
* Think more to coverage the possibiity.  
> Auto Scaling your Concept/Event/Idea.  
  
Event Storming Process => Action | Event => Think About => Final Module.  
  
| Different Layout |  
![Concept Wall](https://i.imgur.com/7BfyA47.jpg)
![Imgur1](https://i.imgur.com/uDfXntp.jpg)
![Imgur2](https://i.imgur.com/s7EwLUG.jpg)
![Imgur3](https://i.imgur.com/L8hGIw2.jpg)
![Imgur4](https://i.imgur.com/ZCitSCo.jpg)
![Imgur5](https://i.imgur.com/RI6VVoF.jpg)
![Imgur6](https://i.imgur.com/BJHYPfq.jpg)
![Imgur7](https://i.imgur.com/rW6df71.jpg)
![Imgur8](https://i.imgur.com/UJ7yNOt.jpg)
  
### *BrainStorming & Idea  
  
![OpenFreePay](https://i.imgur.com/CGG5Dqc.png)  
> OpenFreePay &copy; CopyWrite by Shiame, Krace, MacT and Kevin. All Rights reserved.    
  
* Case Study - Open Coff'ee Shop  
  
Execute the concept from above Layout.  
  
![CoffeeShopConcept](https://i.imgur.com/eVV6Vfz.jpg)
![CoffeeMapFull](https://imgur.com/c2kNMNp)
![CoffeeMapExtand](https://imgur.com/juvgcb0)
![CoffeeMapMarkAPI](https://imgur.com/N1hnD6a)
![CoffeeMap3Party](https://imgur.com/OHrikCB)
![CoffeeMapAPIDefine](https://imgur.com/pIE494A)
  
### Bounded CONTEXT  
  
Bind and Bound out the bordering / Mark down the Limition:  
  
&copy; CopyWrite on this project by Shiame. All Rights reserved. (CC)  