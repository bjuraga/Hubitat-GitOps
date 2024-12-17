# Hubitat-GitOps

A framework to make it easy to extract and apply your own Hubitat configuration. At the moment, in a design stage.

## Design choices
1. Will access the Hubitat hub localy (192.168.0.123), not over internet?
2. Will run locally, maybe in docker?
3. Will be able to extract configuration from Hubitat and store it in config file(s)
4. Will be able to apply configuration from config file(s) to Hubitat
5. Will be able to store backups (reuse the extract functionality)
6. Will not be able to show differences between deployed (running configuration) and the config files
7. Will allow to use diff view between current backup and a selected config in a diff viewer.
8. Will have built in support for Hubitat versions, i.e. if the UI changes in a version it is still possible to write an adapter for the version. Config schema changes should be last resort.
9. Will use an existing web test automation tool. Example: Selenium, Gherkin, Plywright, Puppeteer, etc. Trying Puppeteer.
11. Will support headless mode if applicable. Users will not need to install dev/test tooling. 
12. Will expose humanly readable "code" such that a software development knowledge is not required. Examples: Gherkin ?
13. ?

## Config structure options
1. Follow the UI: Have entities like Hubs, Apps, Child apps, Drivers, Devices
2. Follow the domain: Have entities like Hubs, Rules, Notifications, Devices
3. ?
