# Detect Un-Used AWS IAM Role using AWS RDK, Python boto3
In this, s3 bucket is used to store configuration files.

First clone this repo or copy the py file (detect_unused_iam_roles.py) to your rdk project.
```
git clone https://github.com/SBMagar/unused-iam-role-rdk.git
```

Before deploying, make sure you have successfully setup virtualenv. If you haven't go to project directory and run the following command to create virtualenv: (If you haven't install virtualenv please run **pip install virtualenv**)
```
python -m venv .venv
```

Activate the environment:
```
source .venv/bin/activate
```

Install rdk, boto3 inside activated virtual environment:
```
pip isntall rdk
pip install boto3
```

Now, From project directory initialize rdk:

```
rdk init
```

Now deploy the rule:

```
rdk deploy detect_unused_iam_role_rdk
```

## Resource cleanup
Delete/destroy all the stacks created by rdk:
```
rdk undeploy detect_unused_iam_role_rdk
```

