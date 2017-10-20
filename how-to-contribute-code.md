# How to Contribute Code

Want to help out with the technical side of LouisvilleTech.org?

Great! Here's some things you should know.

## The Basics

We want to do the development in an open source fashion.

The code we accept must be published with an [OSI-approved License](https://opensource.org/licenses), such as [the MIT License](https://opensource.org/licenses/MIT).

We discuss & plan development of the various parts of code in the [#louisvilletech-dev](https://louisville.slack.com/messages/C7DJMQZ5H/) channel.

Participation in development of LouisvilleTech.org related software is subject
to [our Code of Conduct](http://louisvilletech.org/code-of-conduct.html).

## The Site

* [The code for the site is on GitHub](https://github.com/louisvilletech/louisvilletech.org)
* The site runs on a [Ubuntu](https://www.ubuntu.com/) machine in [DigitalOcean](https://www.digitalocean.com/)
* The site is a static site that is generated every 5 minutes via a cron job
* The cron job produces an `dest/events.json` file with all of the aggregated event data.
* The site generation code is written in JavaScript on [Node.js](https://nodejs.org/en/)
* Deployment of the site is automated with [Ansible](https://www.ansible.com/),
  and [the Ansible Playbooks are on GitHub](https://github.com/louisvilletech/louisvilletech.org-ansible)

## Slack Bots

In order for a moderator to install a bot on our Slack Workspace these things need to happen first:

1. The bot must be demonstrated on [the "testing" slack](https://louisvilletechtesting.slack.com)
2. The code for the bot must live under the ["louisvilletech" GitHub organization](https://github.com/louisvilletech)
3. The bot needs to run on either the LouisvilleTech.org server, or a hosted service for which a moderator has an account with appropriate permissions
