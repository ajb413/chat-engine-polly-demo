# PubNub ChatEngine : AWS Polly : Text-To-Speech buttons

Build a chat application with TTS buttons on every chat message.

## Full Tutorial
[Amazon Machine Learning Blog - Build smart chat apps with Amazon machine learning APIs and the PubNub ChatEngine](https://aws.amazon.com/blogs/machine-learning/build-smart-chat-apps-with-amazon-machine-learning-apis-and-the-pubnub-chatengine/)

## Instructions
* Sign up for PubNub
* Sign up for Amazon AWS
* Run [ChatEngine Setup](https://www.pubnub.com/docs/chat-engine/getting-started#automagic-pubnub-setup)
* Get AWS `access` and `secret` keys for Polly guide [here](https://docs.aws.amazon.com/polly/latest/dg/authentication-and-access-control.html)
* Go to the PubNub Functions event handlers in the [admin portal](https://admin.pubnub.com/)
* Add an `On Request` event handler (+ tab) and paste `polly-pfunc.js` contents into the editor
* To the left of the editor, click `MY SECRETS` and add `AWS_access_key` and `AWS_access_key`
* Click `COPY URL` and paste it in `app.js` as `pollyFunctionURI` variable
* Copy the `Publish` and `Subscribe` keys for the app from the admin portal
* Paste them at the top of `app.js`
* Install https://www.npmjs.com/package/http-server or something similar and boot a new server from the root folder of this project
* `http-server`

## Features

There is a Polly TTS button next to every chat bubble!

Uncomment under the `UNCOMMENT` lines in `app.js` to see ChatEngine features like 
* Chat History
* Typing Indicator Plugin 
* Markdown Plugin

![App Screenshot](https://github.com/ajb413/chat-engine-polly-demo/raw/master/screenshot.png "ChatEngine Demo")