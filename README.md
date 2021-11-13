# gitsecret-buildpack
Generates GPG Key and reveals secret files with Git Secret

If you need to reveal your encrypted secrets from [Git Secret](https://git-secret.io) then just load up your GPG key and this buildpack will decrypt the files for you

## Usage

1. Create Config Vars key `GPG_PRIVATE_KEY` and paste the content of GPG Key as is.

The script with generate your GPG as a private_key.gpg and then use it to reveal your secrets.

To add to your application, run:

```
heroku buildpacks:set https://github.com/buyersight/heroku-google-application-credentials-buildpack.git -a your-app-name
```
