anypoint_twitter sms
=======

With a simple webhook from twilio, you can get or set your twitter status and get notified by sms via twilio

prerequisites

1. Anypoint Studio

2. Twilio Connector for anypoint studio (installed through help->install software)

3. Twilio Account

4. Twitter account

You'll need to create a twitter app to obtain all the api keys you need
Important!  Default permissions are read-only, must update to read-write-access direct messages BEFORE generating keys
Follow the "Configure Twitter" example here: http://blogs.mulesoft.org/mule-school-twitter/

Getting started

1. Open the project in mule

2. fill in the mule-app.properties.sample under src/main/app/ the delete .sample from the end of the file name

3. Run the app

Send your twitter status to sms
http://localhost:8081/getstatus

Update your twitter status and send to sms
http://localhost:8081/updateandsms?newstatus=NewStatusGoesHere

Untested Feature since im not hosting publicly and am only using a trial account, therefore I cannot test.
Twilio allows webhooks that can be setup here https://www.twilio.com/user/account/phone-numbers/incoming, so theoretically you could set sms messages to the links above to trigger the events directly from sms.


