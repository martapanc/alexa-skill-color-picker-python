# Alexa Skill - Fav Colour Picker :art:

[Guide](https://github.com/alexa/skill-sample-python-colorpicker)

### Local config

- Download AWS Toolkit plugin for PyCharm
- Set AWS credentials Profile (bottom right on PyCharm)
- Have Docker installed and running

### SAM CLI Installation
```bash
brew tap aws/tap
brew install aws-sam-cli
sam --version
```
[Getting started guide - Hello world](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-getting-started-hello-world.html)
### CL commands
```bash
sam build
sam deploy --guided
sam local invoke -e testEvent.json
```
Once deployed, the ARN code (AWS console > Lambda > Functions > Color picker function > top right corner) needs to be copied and pasted in the Alexa Skill endpoint page.

### Run locally in PyCharm using testEvent.json
- PyCharm should detect a Lambda run configuration - if it doesn't, create one 
- Select testEvent.json as Input file