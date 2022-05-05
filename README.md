# Detect Unused IAM Role using AWS RDK, Python boto3
# s3 bucket is used to store configuration files

First clone this repo or copy the py file (detect_unused_iam_roles.py) to your rdk project.
```
git clone https://github.com/SBMagar/unused-iam-role-rdk.git
```

Go to directory and run:

```
rdk init
```

Now deploy the rule

```
rdk deploy detect_unused_iam_role_rdk
```

## Resource cleanup
Delete/destroy all the stacks created by rdk:
```
rdk undeploy detect_unused_iam_role_rdk
```

