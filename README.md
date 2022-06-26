[![kcemenike](https://circleci.com/gh/kcemenike/autodeploy-project.svg?style=svg)](https://app.circleci.com/pipelines/github/kcemenike/autodeploy-project)

## A complete CI/CD project

This project is a part of the Udacity Cloud DevOps nanodegree and execute the following:

- Explain the fundamentals and benefits of CI/CD to achieve, build, and deploy automation for cloud-based software products.
- Utilize Deployment Strategies to design and build CI/CD pipelines that support Continuous Delivery processes.
- Utilize a configuration management tool to accomplish deployment to cloud-based servers.
- Surface critical server errors for diagnosis using centralized structured logging.

### Instructions

- Fork this repository and clone into your local device
- Connect the repo to your CircleCI account
- Create an S3 bucket that will hold the files in this repo (we will be deploying the repo in this bucket and switching blue to green using cloudfront). Take note of the name of this bucket (in my case, I used udapeople-kelechi1, where `kelechi1` is my workflowID)
- Deploy the cloudfront distribution with the following command, replacing `WorkflowID` with your own bucket suffix  
  `aws cloudformation deploy --template-file .circleci/files/cloudfront.yml --stack-name InitialStack --parameter-overrides WorkflowID=kelechi1`
- push the changes to git to fire up CI pipeline


### Built With 💓

- [Circle CI](www.circleci.com) - Cloud-based CI/CD service
- [Amazon AWS](https://aws.amazon.com/) - Cloud services
- [AWS CLI](https://aws.amazon.com/cli/) - Command-line tool for AWS
- [CloudFormation](https://aws.amazon.com/cloudformation/) - Infrastructure as code
- [Ansible](https://www.ansible.com/) - Configuration management tool
- [Prometheus](https://prometheus.io/) - Monitoring tool

### License

[License](LICENSE.md)
