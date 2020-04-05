## happy path sms prepiad
* start: hi
    - utter_greet
* sms: sms
    - utter_prepaid_postpaid
* prepaid: prepaid
    - utter_prepaid
* custom_plan: custom_plan
    - utter_custom_plan
    - utter_ask_name
* inform: Liku
    - utter_ask_mobile
* inform: 9087654324   <!-- predicted: inform: [9087654324](mobile) -->
    - slot{"mobile": "9087654324"}
    - action_mobile_validation   <!-- predicted: utter_prepaid_postpaid -->
* inform: hello@gmail.com   <!-- predicted: inform: [hello@gmail.com](email) -->
    - slot{"email": "hello@gmail.com"}
    - utter_ack   <!-- predicted: utter_prepaid_postpaid -->


## happy path sms postpaid
* start: hi
    - utter_greet
* sms: sms
    - utter_prepaid_postpaid
* postpaid: prepaid   <!-- predicted: prepaid: prepaid -->
    - utter_postpaid   <!-- predicted: utter_prepaid -->


