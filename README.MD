# AWS CDK + AWS CloudFormation

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

>> CDK uses above structure to look inside the define of "stacks" and knows how to build the structures and apps.  
>>  
>> CDK define APPS in cdk.js, call inside bin/app.ts  
>>  
>> Inside bin/app.ts, it define the enviorment variables.  
>>  
>> <Stack>.ts will be define inside lib/stacks/<name>.ts, tells what infra stacks should be create.  
  
*Clone Template to "Template" Folder*  
  
>> https://docs.aws.amazon.com/ja_jp/cdk/latest/guide/about_examples.html  