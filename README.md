# Go-live checklist
This checklist is used whenever a project is going live at https://programic.com.

## 1. Static files
- [ ] Static files are stored on AWS S3 in the correct region (default eu-central-1).
- [ ] Versioning is enabled on AWS S3.

## 2. Code
- [ ] `composer.lock` and/or `yarn.lock` are present.
- [ ] Traefik labels are properly set up and use middleware `secure-headers` and `maintenance`.

## 3. Services
- [ ] SendGrid is properly set up with a production API key.
- [ ] Pusher is properly set up with a production API key.
- [ ] MessageBird is properly set up with a production API key.
- [ ] Algolia is properly set up with a production API key.
- [ ] Google Cloud is properly set up with a production API key.
- [ ] Amazon Web Services is properly set up with a production API key.

## 4. Dotenv
- [ ] Debug mode is turned off.
- [ ] "From" email address is set correctly.
- [ ] Other .env variables are set correctly?

## 5. Server
- [ ] Production domain points to the correct server.
- [ ] DigitalOcean droplet backups are enabled.
- [ ] Database backups are enabled.

## 6. Pipelines 
- [ ] Bitbucket Pipeline or GitHub actions deploys to production.
- [ ] Assets are built for production.

## 7. Back end
- [ ] Default passwords have been changed.

## 8. Monitoring
- [ ] Crons are monitored by OhDear scheduled tasks.
- [ ] Queue is monitored by OhDear application health.
- [ ] Other OhDear features are set up correctly.
- [ ] Exceptions and logs are caught by Sentry.

## About Programic
Programic is a development agency based in Deventer, The Netherlands. You'll find an overview of all our open source projects [on our GitHub](https://github.com/programic).