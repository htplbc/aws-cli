AWS Command-Line Tools
======================

This directory contains the AWS command-line tools that we're currently using.

It is intended to help us standardize on the same tool set and versions -- dowloading this ish from the AWS developer site, and keeping it up to date, is a pain in the arse.

I place this stuff in `~/.aws-cli` and then add the following to my `.bashrc`:

    export EC2_HOME=~/.aws-cli/ec2
    export AWS_AUTO_SCALING_HOME=~/.aws-cli/as
    export AWS_CLOUDFORMATION_HOME=~/.aws-cli/cfn
    export AWS_CLOUDWATCH_HOME=~/.aws-cli/mon
    export AWS_ELB_HOME=~/.aws-cli/elb
    export AWS_RDS_HOME=~/.aws-cli/rds
    export AWS_IAM_HOME=~/.aws-cli/iam
    export JAVA_HOME=/System/Library/Frameworks/JavaVM.framework/Home/
    export PATH=$PATH:~/.aws-cli/ec2/bin:~/.aws-cli/as/bin:~/.aws-cli/cfn/bin:~/.aws-cli/mon/bin:~/.aws-cli/elb/bin:~/.aws-cli/rds/bin:~/.aws-cli/iam/bin

I also have a separate `~/.aws` directory where I keep credentials files. In my `.bashrc`:

    export EC2_REGION=us-west-1
    export EC2_URL=ec2.us-west-1.amazonaws.com
    export AWS_CREDENTIAL_FILE=~/.aws/bourgeois-bits.credentials
    export EC2_PRIVATE_KEY=~/.aws/pk-XXX.pem
    export EC2_CERT=~/.aws/cert-XXX.pem

-Dave

