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
    - utter_ask_budget
* restaurant_search{"budget": "Lesser than 300"}
    - slot{"budget": "Lesser than 300"}
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
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "chandigarh"}
    - slot{"location": "chandigarh"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "Italian"}
    - slot{"cuisine": "Italian"}
    - utter_ask_budget
* restaurant_search{"budget": "Rs. 300 to 700"}
    - slot{"budget": "Rs. 300 to 700"}
    - action_search_restaurants

## interactive story 1
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "chandigarh"}
    - slot{"location": "chandigarh"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "Rs. 300 to 700"}
    - slot{"budget": "Rs. 300 to 700"}
    - action_search_restaurants
    - slot{"location": "chandigarh"}
    - slot{"response": "New Panna Sweets in SCF 218, Near Fun Republic Cinema, Manimajra, Chandigarh rated 4.1 with avg cost 500 \n\nPal Dhaba in SCO 151, 152, Sector 28 D, Near Sector 28, Chandigarh rated 3.9 with avg cost 650 \n\n"}
    - utter_email
* affirm
    - utter_ask_email
* email_input{"email": "abd@dev.com"}
    - slot{"email": "abd@dev.com"}
    - action_send_mail
    - slot{"email": "abd@dev.com"}
    - utter_mail_confirmation
    - utter_goodbye

## interactive story 2
* greet
    - utter_greet
* restaurant_search{"cuisine": "chinese", "location": "Chandigarh"}
    - slot{"cuisine": "chinese"}
    - slot{"location": "Chandigarh"}
    - utter_ask_budget
* restaurant_search{"budget": "Rs. 300 to 700"}
    - slot{"budget": "Rs. 300 to 700"}
    - action_search_restaurants
    - slot{"location": "Chandigarh"}
    - slot{"response": "Gopal Ji Confectioners in Shop 8, Sector 35 C, Near Sector 35, Chandigarh rated 4.0 with avg cost 350 \n\nPal Dhaba in SCO 151, 152, Sector 28 D, Near Sector 28, Chandigarh rated 3.9 with avg cost 650 \n\n"}
    - utter_email
* deny
    - utter_goodbye

## interactive story 3

* restaurant_search{"budget": "Lesser than 300", "cuisine": "chinese", "location": "gurgaon"}
    - slot{"cuisine": "chinese"}
    - slot{"location": "gurgaon"}
    - slot{"budget": "Lesser than 300"}
    - action_search_restaurants
    - slot{"location": "gurgaon"}
    - slot{"response": "Dilli 6 On Wheels in Shop 84, 85, 86 & 87, HUDA Shopping Complex, Near Medanta Hospital, Sector 32, Near, Sector 31, Gurgaon rated 3.8 with avg cost 250 \n\nBurger Hut in U-6/50, Near Yashwant Department Store, DLF Phase 3, Gurgaon rated 3.6 with avg cost 300 \n\nFomads in U-25/27, Ground Floor, DLF Phase 3, Gurgaon rated 3.6 with avg cost 300 \n\nRao's Meeting Point in Near Omaxe City Center Mall, Sohna Road, Gurgaon rated 3.4 with avg cost 300 \n\nFoodies Nation in U-10/25, DLF phase 3, Gurgaon, Haryana-122001, DLF Phase 3, Gurgaon rated 3.4 with avg cost 300 \n\nHangout Cafe in 16 C, Opposite Lady of Fatima Convent School, New Colony, Old Railway Road, Gurgaon rated 3.4 with avg cost 200 \n\nSuper Bakery in Near Bank of India, Jacobpura, Old Railway Road, Gurgaon rated 3.3 with avg cost 250 \n\nMadras Cafe in SCO 17, Near Huda Office, Sector 14, Gurgaon rated 3.3 with avg cost 300 \n\nIndo Chinese in 178, Ground Floor, Vyapar Kendra, Sushant Lok, Gurgaon rated 3.2 with avg cost 200 \n\nOm Sweets in SCO 141 & 142, Huda Market, Sector 46, Near, Sector 45, Gurgaon rated 3.2 with avg cost 300 \n\n"}
    - utter_email
* email_input{"email": "test@gmail.com"}
    - slot{"email": "test@gmail.com"}
    - action_send_mail
    - slot{"email": "test@gmail.com"}
    - utter_mail_confirmation
    - utter_goodbye


* restaurant_search{"budget": "Lesser than 300", "cuisine": "chinese", "location": "gurgaon"}
    - slot{"cuisine": "chinese"}
    - slot{"location": "gurgaon"}
    - slot{"budget": "Lesser than 300"}
    - slot{"cuisine": "chinese"}
    - slot{"location": "gurgaon"}
    - slot{"budget": "Lesser than 300"}
    - action_search_restaurants
    - slot{"location": "gurgaon"}
    - slot{"response": "Dilli 6 On Wheels in Shop 84, 85, 86 & 87, HUDA Shopping Complex, Near Medanta Hospital, Sector 32, Near, Sector 31, Gurgaon rated 3.8 with avg cost 250 \n\nBurger Hut in U-6/50, Near Yashwant Department Store, DLF Phase 3, Gurgaon rated 3.6 with avg cost 300 \n\nFomads in U-25/27, Ground Floor, DLF Phase 3, Gurgaon rated 3.6 with avg cost 300 \n\nRao's Meeting Point in Near Omaxe City Center Mall, Sohna Road, Gurgaon rated 3.4 with avg cost 300 \n\nFoodies Nation in U-10/25, DLF phase 3, Gurgaon, Haryana-122001, DLF Phase 3, Gurgaon rated 3.4 with avg cost 300 \n\nHangout Cafe in 16 C, Opposite Lady of Fatima Convent School, New Colony, Old Railway Road, Gurgaon rated 3.4 with avg cost 200 \n\nSuper Bakery in Near Bank of India, Jacobpura, Old Railway Road, Gurgaon rated 3.3 with avg cost 250 \n\nMadras Cafe in SCO 17, Near Huda Office, Sector 14, Gurgaon rated 3.3 with avg cost 300 \n\nIndo Chinese in 178, Ground Floor, Vyapar Kendra, Sushant Lok, Gurgaon rated 3.2 with avg cost 200 \n\nOm Sweets in SCO 141 & 142, Huda Market, Sector 46, Near, Sector 45, Gurgaon rated 3.2 with avg cost 300 \n\n"}
    - utter_email
* email_input{"email": "test@gmail.com"}
    - slot{"email": "test@gmail.com"}
    - slot{"email": "test@gmail.com"}
    - action_send_mail
    - slot{"email": "test@gmail.com"}
    - utter_mail_confirmation
    - utter_goodbye
* restaurant_search{"budget": "More than 700", "cuisine": "italian", "location": "mumbai"}
    - slot{"cuisine": "italian"}
    - slot{"location": "mumbai"}
    - slot{"budget": "More than 700"}
    - action_search_restaurants
    - slot{"location": "mumbai"}
    - slot{"response": "The Fusion Kitchen in Shop 1, Opposite Veda Building, Near Bhavdevi Garage, Holy Cross Road, IC colony, Borivali West, Mumbai rated 4.7 with avg cost 1000 \n\nSin City Rooftop Resto & Lounge in 5th Floor, Crystal Point Mall, Andheri Lokhandwala, Andheri West, Mumbai rated 4.6 with avg cost 2500 \n\nAer - Four Seasons in 1/136, E Moses Road, Worli, Mumbai rated 4.6 with avg cost 4500 \n\nJLWA in Unit 1-5, B 40, Patel Commercial Premises, Opposite Citi Mall, Veera Desai Area, Mumbai rated 4.4 with avg cost 2100 \n\nRaasta in 4th & 5th Floor, Rohan Plaza, 5th Road, Near Union Bank, Khar, Mumbai rated 4.3 with avg cost 1500 \n\nTea Villa Cafe in 31, Opposite Globus, Hill Road, Bandra West rated 4.1 with avg cost 1000 \n\nTea Villa Cafe in 28, Aaram Nagar 1, Opposite Dariya Mahal, Versova, Andheri West rated 4.1 with avg cost 1000 \n\nR' ADDA in Ramee Guestline Hotel, 462, A B Nair Road, Juhu, Mumbai rated 4.0 with avg cost 1200 \n\nThe Marina Upper deck - Rooftop Cafe- Sea Palace Hotel in Sea Palace Hotel, PJ Ramchandani Marg, Apollo Bunder, Near Colaba, Mumbai rated 3.9 with avg cost 1600 \n\nTea Villa Cafe in Shop 1& 2, Y-Building, Flower Valley, Opposite Viviana Mall,Eastern Express Highway, Majiwada, Thane West rated 3.9 with avg cost 1000 \n\n"}
    - utter_email
* deny
    - utter_goodbye

