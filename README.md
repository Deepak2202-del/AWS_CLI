# AWS_CLI


# AWS CLI Installation and Configuration Guide (Windows)

Welcome to the AWS CLI installation and configuration guide for Windows. This guide will walk you through the process of installing the AWS CLI on your Windows machine, configuring it, and performing some basic commands to interact with AWS services.

## Installation

To install the AWS CLI on your Windows machine, follow these steps:

1. Download the AWS CLI Installer: You can download the AWS CLI installer from the official AWS website.

2. Run the Installer: Once downloaded, open a command prompt with administrative privileges and run the following command to install AWS CLI:

```bash
msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi
```

If you prefer a silent installation (without any prompts), you can use the following command:

```bash
msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi /qn
```

3. Verify Installation: After the installation is complete, you can verify that the AWS CLI has been installed correctly by running the following command:

```bash
aws --version
```

This should display the version of the AWS CLI installed on your system.

## Configuration

Once the AWS CLI is installed, you need to configure it with your AWS credentials to interact with AWS services. Follow these steps to configure the AWS CLI:

1. Run Configuration Command: Open a command prompt and run the following command:

```bash
aws configure
```

2. Provide Access Key and Secret Key: You will be prompted to enter your AWS Access Key ID and Secret Access Key. These can be obtained from your AWS account's Security Credentials section.

3. Set Default Region: You will also be prompted to set the default region. Enter the AWS region where you want to perform operations.

4. Set Default Output Format (Optional): You can optionally set the default output format. Choose from `json`, `yaml`, `text`, or `table`.

## Basic Commands

Once the AWS CLI is installed and configured, you can start using it to interact with AWS services. Here are some basic commands to get you started:

### List S3 Buckets

To list all the S3 buckets in your AWS account, you can use the following command:

```bash
aws s3 ls
```

### Create EC2 Instance

To create an EC2 instance, you can use the `aws ec2 run-instances` command. Make sure you have the necessary permissions in your AWS account to create EC2 instances.

```bash
aws ec2 run-instances --image-id <AMI-ID> --instance-type <instance-type> --key-name <key-pair-name> --security-group-ids <security-group-id> --subnet-id <subnet-id>
```

Replace `<AMI-ID>`, `<instance-type>`, `<key-pair-name>`, `<security-group-id>`, and `<subnet-id>` with appropriate values.

## Conclusion

Congratulations! You have successfully installed and configured the AWS CLI on your Windows machine. You can now start using the AWS CLI to manage your AWS resources efficiently. For more advanced usage and commands, refer to the [AWS CLI documentation (  https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html )
