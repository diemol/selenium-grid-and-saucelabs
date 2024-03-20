# Extending [Selenium Grid](https://www.selenium.dev/documentation/grid/) with [Sauce Labs](https://saucelabs.com/)

Setting up your Grid can be simple initially. Still, as usage grows and more platforms and browsers are 
needed, you will find yourself in a situation where a more extensive infrastructure needs to be supported. Adding macOS 
and Safari or mobile devices and emulators can be challenging due to the hardware costs and diverse requirements. 
Extending Selenium Grid with Sauce Labs is an excellent solution to add capacity and support more use cases.

Selenium Grid has a Relay feature that enables a local Grid to add Sauce Labs as an extra Node. In this way, Grid 
can enable more coverage to platforms and versions not present locally.

Read more at the Sauce Labs [documentation](https://docs.saucelabs.com/web-apps/automated-testing/selenium/selenium-grid/).

## Implementation Example

This repository uses [GitPod](https://gitpod.io/) to illustrate how to extend your Selenium Grid with Sauce Labs. The
[`.gitpod.yml`](./.gitpod.yml) file configures the environment to download the Grid jar file and start it together with 
the [`config.toml`](./config.toml) file, which configures the Grid Relay feature with the different capabilities you'd
like to use in Sauce Labs.

## Click the button below and see it in action!

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/diemol/selenium-grid-and-saucelabs)

After the Grid is up and running, point your tests at the GitPod URL, and remember to add your `userName` and `accessKey` inside `sauce:options`.




