---
title: "Workshop Cleanup"
chapter: true
weight: 4
---

# Cleaning up of the workshop

The worskshop being launched in your AWS account via AWS Marketplace.

### Please follow the below steps to stop the workshop:

1. Sign in to the AWS Management Console and open the AWS Marketplace console.
2. Go to the Manage subscriptions page.
3. For the delivery method, choose Amazon Machine Image from the dropdown list.
4. Select the subscription for the product that you want to cancel.
5. From the Actions dropdown list, choose Cancel subscription.
6. Read the information provided to Acknowledge that running instances are charged to your account and select the check box. Choose Yes, cancel subscription.
7. Open Manage in AWS Console in a new tab.
8. Terminate the running instance in the Amazon EC2 console. If you have multiple instances running, you must terminate all of them. 
9. Return to the Manage subscriptions tab and choose Yes, Cancel subscription. After canceling your subscription, you lose access to the software and will no longer be billed for it.

### Markdown and Shortcode Resources


### Adding Images and Static Media
Any images and static media to be included in the workshop need to be placed in the `static/images` folder. The format to display an image is as follows: `![Alternate Text](/images/imagename.jpg)` <br>

For example, the markdown for this dog is `![An adorable puppy](/images/dog.jpg)` and the image is in the `static/images` folder. <br>
![An adorable puppy](/images/dog.jpg)

### Creating Links
The format for creating links is `[Link Display Text](http://example.com)`. For example, this link [Hugo Framework](https://gohugo.io/about/what-is-hugo/) was created using `[Hugo Framework](https://gohugo.io/about/what-is-hugo/)`.

### The "More" Menu Section
This section of the menu on the left is designed to add additional resources that are related to the workshop but not necessarily part of the workshop itself. To modify these links, edit the sections marked `[[menu.shortcuts]]` in the `config.toml` located in the root folder. The "name" portion will be what is displayed in the menu. The "url" should be the address of the link. The "weight" setting will adjust the display order, similar to the other "weight" settings utilized in indexes and modules mentioned previously.

### Ensuring Pages Appear In Both Setup Versions
A shortcut to creating the workshop with different setup versions is utilizing the localization functionality of Hugo. By adding a secondary extension to the filename, this file will be included in the specific version of the workshop. Currently, the base utilizes the format `*.ee.md` to signify that the page is to be used in the AWS EventEngine setup. Much of the time, the files will be the same as the content only differs at specific points. It is necessary to add them, however, to make sure that the common content is duplicated across both versions. If you wish to change the secondary extension or default version, this can be done in the `config.toml` file in the heading and `[Languages]` sections.