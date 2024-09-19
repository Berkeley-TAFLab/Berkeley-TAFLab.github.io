---
title: ESP Boat
layout: default
nav_order: 2
---

# ESP Boat

## Description
This iteration of the boat aims to use an ESP32 instead of an Arduino as 
the microcontroller of choice. Furthermore, it is LiPo powered and includes a 
new housing for the electronics. A GUI is used in order to monitor status and visualize
data from the boat. 


## Design Goals 
The design of this particular boat aims to fulfill the following goals:
1. Electronics, especially wiring, should be easier to manage and access. The usage 
of Arduinos with jumpers leads to wires constantly getting pulled out 
2. Power to the system should be delivered by a Lipo instead of the original powerbanks 
to reduce cost. 
3. The microcontroller being used to control these boats should be sufficiently powerful
to manage all the functions it must achieve and for future development as more sensors
are added. 
4. Firmware should be structured cleanly for ease-of-edit and readability 
5. Electronics should have their own isolated environment away from the water that we can 
trust to be safe. 
6. The design of the boat should be cheap, reliable, and easy to reproduce. 

## Sensors
In order for our boat to be autonomous we require the usage of different sensors to 
collect environmental data. 
1. AS5600 Magnetic Encoder - Used in windvane to calculate wind direction 
2. 433 MHz RF Transmitter - Originally used for transmission of operator inputs. 
Deprecated as we opted to use XBees due to the reliability of the Zigbee protocol
as opposed to the protocol-less radios. 
3. XBee Breakout - Used to allow boat to interface with Digi Xbee3 via UART and 
connect to the rest of the mesh network. 
4. MPU6050 IMU - 
5. GTU-7 GPS - Used to track the latitude and longitude of our boat 
6. LISMDL Magnetometer - Used to calculate heading which will be used to determine 
the direction of the boat
7. HW-038 Water Level Sensor - Used to determine if water has breached the boat 



<!-- This is a *bare-minimum* template to create a Jekyll site that uses the [Just the Docs] theme. You can easily set the created site to be published on [GitHub Pages] – the [README] file explains how to do that, along with other details.

If [Jekyll] is installed on your computer, you can also build and preview the created site *locally*. This lets you test changes before committing them, and avoids waiting for GitHub Pages.[^1] And you will be able to deploy your local build to a different platform than GitHub Pages.

More specifically, the created site:

- uses a gem-based approach, i.e. uses a `Gemfile` and loads the `just-the-docs` gem
- uses the [GitHub Pages / Actions workflow] to build and publish the site on GitHub Pages

Other than that, you're free to customize sites that you create with this template, however you like. You can easily change the versions of `just-the-docs` and Jekyll it uses, as well as adding further plugins.

[Browse our documentation][Just the Docs] to learn more about how to use this theme.

To get started with creating a site, simply:

1. click "[use this template]" to create a GitHub repository
2. go to Settings > Pages > Build and deployment > Source, and select GitHub Actions

If you want to maintain your docs in the `docs` directory of an existing project repo, see [Hosting your docs from an existing project repo](https://github.com/just-the-docs/just-the-docs-template/blob/main/README.md#hosting-your-docs-from-an-existing-project-repo) in the template README.

----

[^1]: [It can take up to 10 minutes for changes to your site to publish after you push the changes to GitHub](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll#creating-your-site).

[Just the Docs]: https://just-the-docs.github.io/just-the-docs/
[GitHub Pages]: https://docs.github.com/en/pages
[README]: https://github.com/just-the-docs/just-the-docs-template/blob/main/README.md
[Jekyll]: https://jekyllrb.com
[GitHub Pages / Actions workflow]: https://github.blog/changelog/2022-07-27-github-pages-custom-github-actions-workflows-beta/
[use this template]: https://github.com/just-the-docs/just-the-docs-template/generate -->
