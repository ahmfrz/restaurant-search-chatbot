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


## interactive story 1
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

## interactive story 2
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


## interactive story 3
* restaurant_search{"cuisine": "american"}
    - slot{"cuisine": "american"}
    - utter_ask_location
* restaurant_search{"location": "gurgaon"}
    - slot{"location": "gurgaon"}
    - action_search_restaurants
    - slot{"location": "gurgaon"}
    - slot{"response": "Found Subway in G-6, Central Plaza Mall, Golf Course Road, Gurgaon rated G-6, Central Plaza Mall, Golf Course Road, Gurgaon with avg cost 500 \n\nFound Wildfire - Crowne Plaza in Crowne Plaza, National Highway 8, Sector 29, Gurgaon rated Crowne Plaza, National Highway 8, Sector 29, Gurgaon with avg cost 5000 \n\nFound Fatburger in 102, 1st Floor, Cyber Hub, DLF Cyber City, Gurgaon rated 102, 1st Floor, Cyber Hub, DLF Cyber City, Gurgaon with avg cost 1000 \n\nFound Holy Smoke in 103, 1st Floor, Cyber Hub, DLF Cyber City, Gurgaon rated 103, 1st Floor, Cyber Hub, DLF Cyber City, Gurgaon with avg cost 1800 \n\nFound Sutra Gastropub in 201-202, Cyber Hub, DLF Cyber City, Gurgaon rated 201-202, Cyber Hub, DLF Cyber City, Gurgaon with avg cost 2300 \n\n"}
    - utter_email
* email_input{"email": "test@outlook.com"}
    - slot{"email": "test@outlook.com"}
    - action_send_mail
    - slot{"email": "test@outlook.com"}
    - utter_goodbye


## interactive story 4
* restaurant_search{"location": "amritsar"}
    - slot{"location": "amritsar"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "burmese"}
    - slot{"cuisine": "burmese"}
    - action_search_restaurants
    - utter_goodbye


## interactive story 5
* restaurant_search{"location": "Nashik"}
    - slot{"location": "Nashik"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "Mexican"}
    - slot{"cuisine": "Mexican"}
    - action_search_restaurants
    - slot{"location": "Nashik"}
    - slot{"response": "no results"}
    - utter_goodbye
    

* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "Faridabad"}
    - slot{"location": "Faridabad"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "Italian"}
    - slot{"cuisine": "Italian"}
    - action_search_restaurants
    - slot{"location": "Faridabad"}
    - slot{"response": "Found Oregano India in Shop 2661, Sector 7-10 Market, YMCA Road, Sector 10, Faridabad rated Shop 2661, Sector 7-10 Market, YMCA Road, Sector 10, Faridabad with avg cost 500 \n\nFound Oxy Lounge in Town Park, Opposite District Court, Sector 12, Faridabad rated Town Park, Opposite District Court, Sector 12, Faridabad with avg cost 1500 \n\nFound Cafe Parmesan in 42, 1st Floor, HUDA Market, Sector 15, Faridabad rated 42, 1st Floor, HUDA Market, Sector 15, Faridabad with avg cost 1000 \n\nFound Cafe Grub Up in SCF 43, 2nd Floor, Main Market, Sector 15, Faridabad rated SCF 43, 2nd Floor, Main Market, Sector 15, Faridabad with avg cost 900 \n\nFound Caf Bogchi in SCF 39, First Floor, Above Axis Bank, Sector 15, Faridabad rated SCF 39, First Floor, Above Axis Bank, Sector 15, Faridabad with avg cost 650 \n\n"}
    - utter_email
* deny
    - utter_goodbye
