### Alexa Youtube Music Skill

Alexa does not provide native integration to neither youtube nor youtube music. This skill helps to play music from
youtube music on your amazon echo device

NOTE: The skill will not be published for public use as it can incur charges due to AWS Lambda usage.  Users who
are looking to install this skill on their echo device should have AWS developer account and then use the skill

Anyone is free to publish the skill in their AWS account so that non-tech savvy users can also make use of it. If there
is some skill that is available please raise a PR so that, the link to the skill can be added here

#### Setting up the skill
1. setup aws developer account
2. Setup aws cli and configure, node js is also required
3. Install ask cli and configure
4. `ask deploy` will create lambda functions and deploy
5. Create a project on [https://console.cloud.google.com/apis/dashboard](https://console.cloud.google.com/projectcreate
6. Enable Youtube Data API v3 on https://console.cloud.google.com/apis/dashboard?project=yourprojectname
7. Create an API key (CREATE CREDENTIALS, pick API) on https://console.cloud.google.com/apis/credentials?project=yourprojectname
8. Copy paste the just generated API Key, and add a new Environment Variable named `YOUTUBE_API_KEY` on the Lambda function (click the function https://us-east-1.console.aws.amazon.com/lambda/home?region=us-east-1#/functions/?tab=configure , it's under tab configure)
