## Cloud-Formation nested stacks

### Deploy
```
git clone git@github.com:manujakau/cfn-nested-stacks.git
cd cfn-nested-stacks.git/
cd s3-stored-modules/
s3 cp --recursive . s3://bucket-name
cd ..

Change s3 url's in main.yaml to match with bucket-name.

./deploy [preferd-stack-name-here] [stack-action(create/update)]
```

### Ex:
```
./deploy nested-infra-stack create
```