# AWS Codespace

Setup Codespace for working on AWS.

## Usage

### Credentials

Using IAM Identity Center

```
aws configure sso
```

Once configured, use `--profile` to run commands with different profiles.

### CodeCommit

Support for [CodeCommit GRC](https://docs.aws.amazon.com/codecommit/latest/userguide/setting-up-git-remote-codecommit.html) (git-remote-codecommit) is enabled.

```
git clone codecommit::ap-southeast-1://profile@MyRepo my-repo
```

### CDK

See [CDK getting started](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) for details.

```
python3 -m venv .venv
source .venv/bin/activate
python3 -m pip install -r requirements.txt

deactivate
```