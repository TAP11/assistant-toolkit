# Setting context variables for Watson Assistant web chat

**For a full walk through of how this code works, please visit the [tutorial page](https://cloud.ibm.com/docs/watson-assistant?topic=watson-assistant-web-chat-develop-set-context) in the Watson Assistant documentation.**

This code is for extending the Watson Assistant web chat. If you are new to developing with web chat, please start with the [web chat development overview](https://cloud.ibm.com/docs/watson-assistant?topic=watson-assistant-web-chat-develop). The code in this folder is commented with links and references to the web chat APIs used.

This example demonstrates how to set variables using context so those variables are available within an action.

It demonstrates:

- How to use a [**pre:send**](https://web-chat.global.assistant.watson.cloud.ibm.com/docs.html?to=api-events#presend) event handler to set a context variable when a message is sent.
- How to use a variable in an action.

## Running the Code

### Running the JavaScript Example

- Open the [client/javascript/index.html](client/javascript/index.html) file in a web browser.
- Open web chat and you should see a greeting message customized with a user's name.

## Setting up your own assistant

This example is configured to use an existing assistant set up for common use by anyone running this example. If you want to set up your own assistant, you'll need to perform the steps below.

- Import the [actions.json](actions.json) file located in the repository for this example into your assistant.
- Modify the `integrationID`, `region`, `serviceInstanceID` and `subscriptionID` (only for enterprise accounts) in the `watsonAssistantChatOptions` used in this example to match those in the web chat embed code for your assistant.