# twilio

A simple python code to send text messages from twilio account to the registered phone number using the module called Twilio which is a third-party module and installed separetely using pip.

Here, the twilio accountSID and authentication_token is used as the username and password to login 
  create() function tells the Twilio's server to send the specified message to the respective number. 
  The create() returns an object which has various attributes such as,
   - message.status
   - message.date_created
   - message.date_sent
   - message.sid

we can check the current status by doing,
  updatedMessage = client.messages.get(message.sid)
  - updatedMessage.status // returns the updated status whether message delivered
