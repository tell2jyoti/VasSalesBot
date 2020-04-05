#### This file contains tests to evaluate that your bot behaves as expected. 
#### If you want to learn more, please see the docs: https://rasa.com/docs/rasa/user-guide/evaluating-models/

## happy path sms prepiad
* start: hi
  - utter_greet
* sms: sms
  - utter_prepaid_postpaid
* prepaid: prepaid
 - utter_prepaid
* custom_plan:custom_plan
 - utter_custom_plan
 - utter_ask_name
* inform{"name": "Jyoti"}: Liku
 - utter_ask_mobile
* inform{"mobile": "9876543210"}: 9087654324
 - action_mobile_validation
* inform{"email": "test@example.com"}:hello@gmail.com
 - utter_ack

## happy path sms postpaid
* start: hi
  - utter_greet
* sms: sms
  - utter_prepaid_postpaid
* postpaid: prepaid
 - utter_postpaid