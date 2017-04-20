Language Translator Node-RED Bluemix Demo Application
====================================

### Node-RED in BlueMix

This repository is a Node-RED application that has a default flow for Language Translation.
It can be deployed into Bluemix with only a couple clicks. Try it out for yourself right now by clicking:

[![Deploy to Bluemix](https://bluemix.net/deploy/button.png)](https://bluemix.net/deploy?repository=https://github.com/ValerieLampkin/node-red-bluemix-starter.git)

### How does this work?

When you click the button, you are taken to Bluemix where you get a pick a name
for your application at which point the platform takes over, grabs the code from
this repository and gets it deployed.

It will automatically create an instance of the Cloudant service, call it
`sample-node-red-cloudantNoSQLDB` and bind it to you app. This is where your
Node-RED instance will store its data. If you deploy multiple instances of
Node-RED from this repository, they will share the one Cloudant instance.

It includes a default flow that is automatically deployed the first time
Node-RED runs.

### Customising Node-RED

This repository is here to be cloned, modified and re-used to allow anyone create
their own Node-RED based application that can be quickly deployed to Bluemix.

The default flows are stored in the `defaults` directory in the file called `flow.json`.
When the application is first started, this flow is copied to the attached Cloudant
instance. When a change is deployed from the editor, the version in cloudant will
be updated - not this file.

The web content you get when you go to the application's URL is stored under the
`public` directory.

Additional nodes can be added to the `package.json` file and all other Node-RED
configuration settings can be set in `bluemix-settings.js`.

If you do clone this repository, make sure you update this `README.md` file to point
the `Deploy to Bluemix` button at your repository.

If you want to change the name of the Cloudant instance that gets created, the memory
allocated to the application or other deploy-time options, have a look in `manifest.yml`.

### DISCLAIMER

IBM DOES NOT WARRANT OR REPRESENT THAT THE CODE PROVIDED IS COMPLETE OR UP-TO-DATE.  IBM DOES NOT WARRANT,  REPRESENT OR IMPLY RELIABILITY, SERVICEABILITY OR FUNCTION OF THE CODE.  IBM IS UNDER NO OBLIGATION TO UPDATE  CONTENT NOR PROVIDE FURTHER SUPPORT.  

ALL CODE IS PROVIDED "AS IS," WITH NO WARRANTIES OR GUARANTEES WHATSOEVER.  IBM EXPRESSLY DISCLAIMS TO THE  FULLEST EXTENT PERMITTED BY LAW ALL EXPRESS, IMPLIED,  STATUTORY AND OTHER WARRANTIES, GUARANTEES, OR  REPRESENTATIONS, INCLUDING, WITHOUT LIMITATION, THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR  PURPOSE, AND NON-INFRINGEMENT OF PROPRIETARY AND INTELLECTUAL PROPERTY RIGHTS.  YOU UNDERSTAND AND AGREE THAT  YOU USE THESE MATERIALS, INFORMATION, PRODUCTS, SOFTWARE, PROGRAMS, AND SERVICES, AT YOUR OWN DISCRETION AND  RISK AND THAT YOU WILL BE SOLELY RESPONSIBLE FOR ANY DAMAGES THAT MAY RESULT, INCLUDING LOSS OF DATA OR DAMAGE TO YOUR COMPUTER SYSTEM.

IN NO EVENT WILL IBM BE LIABLE TO ANY PARTY FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY OR  CONSEQUENTIAL DAMAGES OF ANY TYPE WHATSOEVER RELATED TO OR ARISING FROM USE OF THE CODE FOUND HEREIN, WITHOUT  LIMITATION, ANY LOST PROFITS, BUSINESS INTERRUPTION, LOST SAVINGS, LOSS OF PROGRAMS OR OTHER DATA, EVEN IF IBM IS EXPRESSLY ADVISED OF THE POSSIBILITY OF SUCH DAMAGES. THIS EXCLUSION AND WAIVER OF LIABILITY APPLIES TO ALL CAUSES OF ACTION, WHETHER BASED ON CONTRACT, WARRANTY, TORT OR ANY OTHER LEGAL THEORIES.

COPYRIGHT LICENSE:
THIS INFORMATION CONTAINS SAMPLE APPLICATION PROGRAMS IN SOURCE LANGUAGE, WHICH ILLUSTRATE PROGRAMMING TECHNIQUES ON VARIOUS OPERATING PLATFORMS. YOU MAY COPY, MODIFY, AND DISTRIBUTE THESE SAMPLE PROGRAMS IN ANY FORM WITHOUT PAYMENT TO IBM, FOR THE PURPOSES OF DEVELOPING, USING, MARKETING OR DISTRIBUTING APPLICATION PROGRAMS CONFORMING TO THE APPLICATION PROGRAMMING INTERFACE FOR THE OPERATING PLATFORM FOR WHICH THE SAMPLE PROGRAMS ARE WRITTEN. THESE EXAMPLES HAVE NOT BEEN THOROUGHLY TESTED UNDER ALL CONDITIONS. IBM, THEREFORE, CANNOT GUARANTEE OR IMPLY RELIABILITY, SERVICEABILITY, OR FUNCTION OF THESE PROGRAMS. THE SAMPLE PROGRAMS ARE PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND. IBM SHALL NOT BE LIABLE FOR ANY DAMAGES ARISING OUT OF YOUR USE OF THE SAMPLE PROGRAMS.
