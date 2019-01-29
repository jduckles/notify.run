# Serverless Setup Instructions

1. Setup serverless: https://serverless.com/framework/docs/providers/aws/guide/quick-start/
2. Then you'll need to generate a public/private key pair using the vapid python library, instructions at: https://github.com/web-push-libs/vapid/tree/master/python
3. Create a `.env.prod` file with the following values set:
```
NOTIFY_VAPID_PRIVKEY= # From step 2
NOTIFY_VAPID_PUBKEY= # From step 2
NOTIFY_VAPID_EMAIL= # Some contact email of form 'mailto:me@here.org'
NOTIFY_API_SERVER= 
NOTIFY_WEB_SERVER= 
```
4. `./deploy.sh`
