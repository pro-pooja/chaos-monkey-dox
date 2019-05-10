# chaos-monkey-dox
This repo contains the steps to re-create an application running on Heroku server (along with all the addons), on another Heroku app.


## Table of contents:
* [Github setup](https://github.com/jdecode/chaos-monkey-dox/blob/master/github.md)
    * [Signup/Login](https://github.com/jdecode/chaos-monkey-dox/blob/master/github.md#loginsignup-on-github)
    * [Create repo](https://github.com/jdecode/chaos-monkey-dox/blob/master/github.md#create-new-repository)
    * Create team
    * Assign members to team
    * [Push Local code to repo](https://github.com/jdecode/chaos-monkey-dox/blob/master/github.md#push-local-code-to-repo)
* [Heroku setup](https://github.com/jdecode/chaos-monkey-dox/blob/master/heroku.md)
    * [Register / Login](https://github.com/jdecode/chaos-monkey-dox/blob/master/heroku.md#loginsignup-heroku)
    * [Connect credit/debit card](https://github.com/jdecode/chaos-monkey-dox/blob/master/heroku.md#connect-creditdebit-card-optional)
    * [Create 2 apps (UAT/Prod)](https://github.com/jdecode/chaos-monkey-dox/blob/master/heroku.md#create-2-apps-uatprod)
    * [Create a pipeline](https://github.com/jdecode/chaos-monkey-dox/blob/master/heroku.md#addattach-apps-to-pipeline)
    * [Add/Attach apps to pipeline](https://github.com/jdecode/chaos-monkey-dox/blob/master/heroku.md#addattach-apps-to-pipeline)
    * [Configure addons (explain)](https://github.com/jdecode/chaos-monkey-dox/blob/master/heroku.md#configure-addons-explain)
    * [Add ENV variables](https://github.com/jdecode/chaos-monkey-dox/blob/master/heroku.md#add-env-variables)
    * [Add Procfile](https://github.com/jdecode/chaos-monkey-dox/blob/master/heroku.md#add-procfile)
    * [Register/Add domain name](https://github.com/jdecode/chaos-monkey-dox/blob/master/heroku.md#registeradd-domain-name)
        * [Add PointDNS](https://github.com/jdecode/chaos-monkey-dox/blob/master/heroku.md#add-pointdns)
        * [Add DNS records](https://github.com/jdecode/chaos-monkey-dox/blob/master/heroku.md#add-dns-records)
    * [Generate/Configure SSL certificate](https://github.com/jdecode/chaos-monkey-dox/blob/master/heroku.md#generateconfigure-ssl-certificate)
* [Circle CI](https://github.com/jdecode/chaos-monkey-dox/blob/master/circleci.md#circleci-setup)
    * [Login/Signup](https://github.com/jdecode/chaos-monkey-dox/blob/master/circleci.md#loginsignup)
    * [Project Setup](https://github.com/jdecode/chaos-monkey-dox/blob/master/circleci.md#project-setup)
    * [CircleCI configuration](https://github.com/jdecode/chaos-monkey-dox/blob/master/circleci.md#circleci-configuration) i.e. config.yml
    * [Add ENV variables](https://github.com/jdecode/chaos-monkey-dox/blob/master/circleci.md#add-env-variables)
* [Rollbar](https://github.com/jdecode/chaos-monkey-dox/blob/master/rollbar.md)
    * [Setup](https://github.com/jdecode/chaos-monkey-dox/blob/master/rollbar.md#setup)
    * [Integrate with Trello and Slack](https://github.com/jdecode/chaos-monkey-dox/blob/master/rollbar.md#integrate-with-trello-and-slack)
        * [Slack](https://github.com/jdecode/chaos-monkey-dox/blob/master/rollbar.md#slack)
        * [Trello](https://github.com/jdecode/chaos-monkey-dox/blob/master/rollbar.md#trello)
    * [Generate and Verify Error reporting](https://github.com/jdecode/chaos-monkey-dox/blob/master/rollbar.md#generate-and-verify-error-reporting)
* [New Relic](https://github.com/jdecode/chaos-monkey-dox/blob/master/newrelic.md)
    * [Setup](https://github.com/jdecode/chaos-monkey-dox/blob/master/newrelic.md#setup)
    * [View Performance Data](https://github.com/jdecode/chaos-monkey-dox/blob/master/newrelic.md#view-performance-data)
    * [Alert for High Apdex Score](https://github.com/jdecode/chaos-monkey-dox/blob/master/newrelic.md#alert-for-high-apdex-score)
* [Papertrail](https://github.com/jdecode/chaos-monkey-dox/blob/master/papertrail.md)
    * [Setup](https://github.com/jdecode/chaos-monkey-dox/blob/master/papertrail.md#setup)
    * [Event Viewer](https://github.com/jdecode/chaos-monkey-dox/blob/master/papertrail.md#event-viewer)
    * [Search](https://github.com/jdecode/chaos-monkey-dox/blob/master/papertrail.md#search)
    * [Save Searches](https://github.com/jdecode/chaos-monkey-dox/blob/master/papertrail.md#save-searches)
    * [Create Events Alerts](https://github.com/jdecode/chaos-monkey-dox/blob/master/papertrail.md#create-events-alerts)
* [Pre-Commit Hooks](https://github.com/jdecode/chaos-monkey-dox/blob/master/pre-commit.md)
    * CodeSniffer
    * MessDetector
    * PHPUnit/TDD