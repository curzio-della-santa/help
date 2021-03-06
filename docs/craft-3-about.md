---

template:         article
reviewed:         2020-08-20
title:            About Craft on fortrabbit
naviTitle:        About Craft on fortrabbit
order:            1
lead:             Craft 3 is the CMS you and your clients will love. We love it too. Our aim is to help you — the developer — to successfully develop and deploy Craft here. This is your entry point. 
group:            craft
stack:            all

websiteLink:      https://craftcms.com/
websiteLinkText:  craftcms.com
category:         CMS
image:            craft-cms-mark-black-new.svg
version:          3.5
supportLevel:     a

keywords:
  - craft
  - craftCMS
  - setup
  - Professional
  - Universal

---

## Choose your Stack

There are [two hosting stacks](/stacks) here on fortrabbit. You can choose with each new [App](/app) your create:

1. The [Universal Stack](/app-uni) has VPS or shared hosting feeling. It's easy to use, affordable, but limited in scaling. Use it for testing + small projects.
2. The [Professional Stack](/app-pro) is designed to scale horizontally. All components are redundant to assure high uptime. Use it for serious business + potentially large sites. 


## Choose your workflow

There are many ways to work with Craft CMS — depending on project needs and skills.

### Modern workflow

Experienced developers who are ready to work with a terminal, [Git](/git) and [Composer](/composer) will benefit most from our advanced workflows. This is where our 💜s are.

1. **[Install Craft CMS locally](craft-3-install-local)**: Install new with Composer or use an existing project
2. **[Setup Craft for fortrabbit](/craft-3-setup)**: Prepare environments, sync database
3. **[Deploy Craft with Git](/craft-3-deploy-git)**
4. **Manage assets** for [Uni Apps](/craft-3-assets-uni) or [Pro Apps](/craft-3-assets-pro)
5. **[Tune Craft](/craft-3-tune)**: Master it!


### Craft Copy

**Take a shortcut!** We have published this little handy open-source command line tool to speed up common deployment tasks around Craft CMS on fortrabbit. It connects your local Craft CMS installation with an App on fortrabbit and then enables you to sync database and assets in a speedy and convenient way. It guides you through the process of setting everything up, and it even has a table to show you which parts are still missing. Give it a try! Here is an appetizer:

```bash
# Install and initialize
$ composer config platform --unset
$ composer require fortrabbit/craft-copy:^1.0.0-RC11
$ ./craft plugin/install copy
$ ./craft copy/setup

# Sync database up (local ⟶ fortrabbit)
$ php craft copy/db/up
```

Please head on to [github.com/fortrabbit/craft-copy](https://github.com/fortrabbit/craft-copy) for more details and usage examples.


### Legacy workflow

Developers focusing on front-end or web designers are likely more comfortable using the legacy SFTP workflow. Use this workflow when you are coming from WordPress or if you are not comfortable with a terminal, Git and Composer. This is your route:

1. **[Install Craft CMS locally](craft-3-install-local)**: Install new with Composer or use an existing project
2. **[Setup Craft for fortrabbit](/craft-3-setup)**: Prepare environments, sync database
3. **[Upload Craft with SFTP](/craft-3-upload-sftp)**
4. **[Tune Craft](/craft-3-tune)**: Master it!
