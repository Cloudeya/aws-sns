# Amazon Simple Notification Service (SNS)

This template describes a SNS topic that can be used by many other templates to receive alerts. You can add one or multiple subscribers to this topic and they will all receive the same alerts. Supported transports are:

* Email
* HTTP endpoint
* HTTPS endpoint (can be used by [Slack Incoming Webhooks](https://api.slack.com/incoming-webhooks))

![Architecture](./images/aws-sns.png?raw=true "Architecture")

## Slack Incoming WebHooks Configuration

![Slack](./images/slack.png?raw=true "Slack Incoming Webhooks")

1\. You need to create a new channel to receive SNS notifications (e.g., aws-sns).

2\. Next, configure Slack Integrations. Typically, this is available [here](https://update-this-with-your-domain-name.slack.com/services/new):

![Slack Incoming Webhooks](./images/slack-webhook1.png?raw=true "Slack Incoming Webhooks")

3\. Select the appropriate Slack channel to integrate a new Incoming WebHooks:

![Slack Incoming Webhooks](./images/slack-webhook2.png?raw=true "Slack Incoming Webhooks")

4\. You'll be presented with **Setup Instructions** and **Webhook URL** after adding the integration:

![Slack Incoming Webhooks](./images/slack-webhook3.png?raw=true "Slack Incoming Webhooks")

5\. That's it! You’re done configuring Slack! Click the button below to launch the stack and don't forget to supply your Webhook URL as you go through the installation.

## Installation Guide

1. [![Launch Stack](./images/launch-stack.png)](https://console.aws.amazon.com/cloudformation/home#/stacks/new?stackName=aws-sns&templateURL=https://raw.githubusercontent.com/Cloudeya/aws-sns/master/aws-sns.json)
1. Click **Next** to proceed with the next step of the wizard.
1. Specify a name and all parameters for the stack.
1. Click **Next** to proceed with the next step of the wizard.
1. Click **Next** to skip the **Options** step of the wizard.
1. Check the **I acknowledge that this template might cause AWS CloudFormation to create IAM resources.** checkbox.
1. Click **Create** to start the creation of the stack.
1. Wait until the stack reaches the state **CREATE_COMPLETE**

## Support

We help startups, private equity and Government Digital Service (GDS) build successful products by solving challenging problems through design thinking, intuitive interfaces, and software engineering; we use the latest easy to scale technologies. Additionally, we offer paid support for our CloudFormation templates. Our team can set up cloud resources based on our templates, create custom templates for specific use cases, and resolve existing issues in production environments. Ready to start? [Hire us](mailto:cloudeya@pm.me?subject=Cloud%20Infrastructure).

## License

The script is published under [BSD 3-Clause License](license.txt).

## Copyright

(c) 2018 [Cloudeya Limited](https://www.cloudeya.ml).
