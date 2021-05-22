## complete path
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "delhi"}
    - slot{"location": "delhi"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - action_search_restaurants
    - slot{"location": "delhi", "response": "Found "}
    - utter_email
* affirm
    - utter_ask_email
* email_input{"email":"abcd@gmail.com"}
    - slot{"email": "abcd@gmail.com"}
    - action_send_mail
    - utter_mail_confirmation
    - utter_goodbye

## location specified
* greet
    - utter_greet
* restaurant_search{"location": "delhi"}
    - slot{"location": "delhi"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - action_search_restaurants
* affirm
    - utter_goodbye



* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "egypt"}
    - slot{"location": "egypt"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - action_search_restaurants
    - utter_goodbye

* restaurant_search{"location": "delhi", "cuisine": "mexican"}
    - slot{"cuisine": "mexican"}
    - slot{"location": "delhi"}
    - action_search_restaurants
    - slot{"location": "delhi"}
    - slot{"response": "Found Blues in N-18, Outer Circle, Opposite Katurbha Gandhi Marg, Connaught Place, New Delhi rated N-18, Outer Circle, Opposite Katurbha Gandhi Marg, Connaught Place, New Delhi with avg cost 1100 \n\nFound FLYP@MTV in N/57 & N/60, 1st Floor, Outer Circle, Connaught Place, New Delhi rated N/57 & N/60, 1st Floor, Outer Circle, Connaught Place, New Delhi with avg cost 1200 \n\nFound Kinbuck 2 in P-10/90, 1st & 2nd Floor, Outer Circle, Connaught Place, New Delhi rated P-10/90, 1st & 2nd Floor, Outer Circle, Connaught Place, New Delhi with avg cost 1600 \n\nFound Moets Arabica in N-20, Outer Circle, Connaught Place, New Delhi rated N-20, Outer Circle, Connaught Place, New Delhi with avg cost 400 \n\nFound Oh My God in 14-15, 2nd Floor, Block F, Inner Circle, Connaught Place, New Delhi rated 14-15, 2nd Floor, Block F, Inner Circle, Connaught Place, New Delhi with avg cost 1400 \n\n"}
    - utter_email
* email_input{"email": "hello@ymail.com"}
    - slot{"email": "hello@ymail.com"}
    - action_send_mail
    - utter_mail_confirmation
    - utter_goodbye
