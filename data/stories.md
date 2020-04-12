## happy path sms prepiad
* start
  - utter_greet
* sms
  - utter_prepaid_postpaid
* prepaid
 - utter_prepaid
* custom_plan
 - utter_custom_plan
 - utter_ask_name
* inform{"name": "Jyoti"}
 - utter_ask_mobile
* inform{"mobile": "9876543210"}
 - action_mobile_validation
* inform{"email": "test@example.com"}
 - utter_ack
 - action_restart

## happy path sms postpaid
* start
  - utter_greet
* sms
  - utter_prepaid_postpaid
* postpaid
  - utter_postpaid
* custom_plan
  - utter_custom_plan
  - utter_ask_name
* inform{"name": "Jyoti"}
  - utter_ask_mobile
* inform{"mobile": "9876543210"}
  - action_mobile_validation
* inform{"email": "test@example.com"}
  - utter_ack
  - action_restart

## happy path ivr prepaid
* start
 - utter_greet
* ivr
 - utter_prepaid_postpaid
* prepaid
 - utter_prepaid
* custom_plan
 - utter_custom_plan
 - utter_ask_name
* inform{"name": "Jyoti"}
 - utter_ask_mobile
* inform{"mobile": "9876543210"}
 - action_mobile_validation
* inform{"email": "test@example.com"}
 - utter_ack
 - action_restart

## happy path Ivr postpaid
* start
  - utter_greet
* sms
  - utter_prepaid_postpaid
* postpaid
  - utter_postpaid
* custom_plan
  - utter_custom_plan
  - utter_ask_name
* inform{"name": "Jyoti"}
  - utter_ask_mobile
* inform{"mobile": "9876543210"}
  - action_mobile_validation
* inform{"email": "test@example.com"}
  - utter_ack
  - action_restart