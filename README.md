# Test-at-scale

Contains scripts to setup TAS.

- Laser <https://github.com/LambdaTest/laser>
- Photon <https://github.com/LambdaTest/photon>
- Neuron <https://github.com/LambdaTest/neuron>
- JS Runners <https://github.com/LambdaTest/test-at-scale-js>
- Test-at-Scale <https://github.com/LambdaTest/test-at-scale>
- Test-at-Scale-js-smart-select <https://github.com/LambdaTest/test-at-scale-js-smart-select>

## Dev Onboarding

### Local System Setup

#### Mac Users

- Install [Homebrew](https://brew.sh/).

```bash
/bin/bash -c "$(curl -fsSL <https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh>)"
```

- Install [Docker Desktop](https://www.docker.com/products/docker-desktop). Start the Docker Desktop Application before proceeding further.

- Add your machine’s [SSH keys on GitHub](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

- Create a new folder and paste mac_deployer.sh (refer Attachments) in that folder.

- Run the script using the command below. (You'll need to define credentials for various services and configurations of resources required by TestAtScale system)

```bash
bash mac_deployer.sh
```

**This script may ask for your root password in order to add entry in /etc/hosts.**

### Enviroment variables

```bash
db_pass=db-pass
azure_acc_name=azure-acc-name
azure_acc_key=azure-acc-key
github_client_id=github-client-id
github_client_secret=github-client-secret
gitlab_client_id=gitlab-client-id
gitlab_client_secret=gitlab-client-secret
bitbucket_client_id=bitbucket-client-id
bitbucket_client_secret=bitbucket-client-secret
github_app_app_name=github-app-app-id
github_app_app_id=github-app-app-id
github_app_client_id=github-app-client-id
github_app_client_secret=github-app-client-secret
github_app_private_key=github-app-private-key
```
#### Obtaining the values for environment variables

- db_pass: This is the password for the database. You can use any password you want. This password will be used to connect to the database running in a mysql docker container locally from the application.

- azure_acc_name: This is the name of the Azure account. You can find this in the Azure portal.

- azure_acc_key: This is the key of the Azure account. You can find this in the Azure portal.

- github_client_id: This is the client id of the GitHub application. You can find this in the GitHub application settings. View more at <https://docs.github.com/en/developers/apps/building-oauth-apps/creating-an-oauth-app>

- github_client_secret: This is the client secret of the GitHub application. You can find this in the GitHub application settings. View more at <https://docs.github.com/en/developers/apps/building-oauth-apps/creating-an-oauth-app>

- gitlab_client_id: This is the client id of the GitLab application. You can find this in the GitLab application settings. View more at <https://docs.gitlab.com/ee/integration/oauth_provider.html>

- gitlab_client_secret: This is the client secret of the GitLab application. You can find this in the GitLab application settings. View more at <https://docs.gitlab.com/ee/integration/oauth_provider.html>

- bitbucket_client_id: This is the client id of the Bitbucket application. You can find this in the Bitbucket application settings. View more at <https://developer.atlassian.com/cloud/bitbucket/oauth-2/>

- bitbucket_client_secret: This is the client secret of the Bitbucket application. You can find this in the Bitbucket application settings. View more at <https://developer.atlassian.com/cloud/bitbucket/oauth-2/>

- github_app_app_name: This is the name of the GitHub application. You can find this in the GitHub application settings. View more at <https://docs.github.com/en/developers/apps/building-github-apps/creating-a-github-app>

- github_app_app_id: This is the app id of the GitHub application. You can find this in the GitHub application settings. View more at <https://docs.github.com/en/developers/apps/building-github-apps/creating-a-github-app>

- github_app_client_id: This is the client id of the GitHub application. You can find this in the GitHub application settings. View more at <https://docs.github.com/en/developers/apps/building-github-apps/creating-a-github-app>

- github_app_client_secret: This is the client secret of the GitHub application. You can find this in the GitHub application settings. View more at <https://docs.github.com/en/developers/apps/building-github-apps/creating-a-github-app>

- github_app_private_key: This is the private key of the GitHub application. You can find this in the GitHub application settings. View more at <https://docs.github.com/en/developers/apps/building-github-apps/creating-a-github-app>

 
