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


* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "bangalore"}
    - slot{"location": "bangalore"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "Lesser than 300"}
    - slot{"budget": "Lesser than 300"}
    - action_search_restaurants
    - slot{"location": "bangalore"}
    - slot{"response": ""}
    - utter_goodbye
* restaurant_search{"location": "tata"}
    - slot{"location": "tata"}

* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "bangalore"}
    - slot{"location": "bangalore"}
    - slot{"location": "bangalore"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "Lesser than 300"}
    - slot{"budget": "Lesser than 300"}
    - slot{"budget": "Lesser than 300"}
    - action_search_restaurants
    - slot{"location": "bangalore"}
    - slot{"response": ""}
    - utter_goodbye
* restaurant_search{"location": "rishikesh"}
    - slot{"location": "rishikesh"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - action_search_restaurants
    - utter_goodbye
* goodbye

* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "bangalore"}
    - slot{"location": "bangalore"}
    - slot{"location": "bangalore"}
    - slot{"location": "bangalore"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "Lesser than 300"}
    - slot{"budget": "Lesser than 300"}
    - slot{"budget": "Lesser than 300"}
    - slot{"budget": "Lesser than 300"}
    - action_search_restaurants
    - slot{"location": "bangalore"}
    - slot{"response": ""}
    - utter_goodbye
* restaurant_search{"location": "rishikesh"}
    - slot{"location": "rishikesh"}
    - slot{"location": "rishikesh"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - action_search_restaurants
    - utter_goodbye
* restaurant_search{"location": "faridabad"}
    - slot{"location": "faridabad"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - action_search_restaurants
    - slot{"location": "faridabad"}
    - slot{"response": "Shree Rathnam in LG-28, Crown Plaza Mall, Sector 15-A, Sector 15, Faridabad rated 3.4 with avg cost 800 \n\nShree Rathnam in Ground Floor, Ridhi Sidhi Plaza, Ashoka Main, Sector 34, Faridabad rated 2.7 with avg cost 800 \n\n"}
    - utter_email
* affirm
    - utter_ask_email
* email_input{"email": "kritka.ag@ymail.com"}
    - slot{"email": "kritka.ag@ymail.com"}
    - action_send_mail
    - slot{"email": "kritka.ag@ymail.com"}
    - utter_mail_confirmation
    - utter_goodbye
* affirm

* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "bangalore"}
    - slot{"location": "bangalore"}
    - slot{"location": "bangalore"}
    - slot{"location": "bangalore"}
    - slot{"location": "bangalore"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "Lesser than 300"}
    - slot{"budget": "Lesser than 300"}
    - slot{"budget": "Lesser than 300"}
    - slot{"budget": "Lesser than 300"}
    - slot{"budget": "Lesser than 300"}
    - action_search_restaurants
    - slot{"location": "bangalore"}
    - slot{"response": ""}
    - utter_goodbye
* restaurant_search{"location": "rishikesh"}
    - slot{"location": "rishikesh"}
    - slot{"location": "rishikesh"}
    - slot{"location": "rishikesh"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - action_search_restaurants
    - utter_goodbye
* restaurant_search{"location": "faridabad"}
    - slot{"location": "faridabad"}
    - slot{"location": "faridabad"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - action_search_restaurants
    - slot{"location": "faridabad"}
    - slot{"response": "Shree Rathnam in LG-28, Crown Plaza Mall, Sector 15-A, Sector 15, Faridabad rated 3.4 with avg cost 800 \n\nShree Rathnam in Ground Floor, Ridhi Sidhi Plaza, Ashoka Main, Sector 34, Faridabad rated 2.7 with avg cost 800 \n\n"}
    - utter_email
* affirm
    - utter_ask_email
* email_input{"email": "kritka.ag@ymail.com"}
    - slot{"email": "kritka.ag@ymail.com"}
    - slot{"email": "kritka.ag@ymail.com"}
    - action_send_mail
    - slot{"email": "kritka.ag@ymail.com"}
    - utter_mail_confirmation
    - utter_goodbye
* restaurant_search{"budget": "Lesser than 300", "cuisine": "american", "location": "Nashik"}
    - slot{"cuisine": "american"}
    - slot{"location": "Nashik"}
    - slot{"budget": "Lesser than 300"}
    - action_search_restaurants
    - slot{"location": "Nashik"}
    - slot{"response": ""}
    - utter_goodbye

* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "Ahmedabad"}
    - slot{"location": "Ahmedabad"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - utter_ask_budget
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - action_search_restaurants
    - slot{"location": "Ahmedabad"}
    - slot{"response": "Lollo Rosso in Shop 2, Ground Floor, Aeon Complex, Opposite Navkar Institute, Navrangpura, Ahmedabad rated 4.6 with avg cost 1000 \n\nBrick Kitchen in At Five Petals Hotel & Banquets, Near Chanakyapuri Bridge, Ghatlodia, Ahmedabad rated 4.3 with avg cost 900 \n\n650 - The Global Kitchen in Shreekunj Mandapam, Beside Golden Tulip Bunglows & Tulip Citadel, Manekbaug, Ambavadi, Ahmedabad rated 4.2 with avg cost 900 \n\nBrick Kitchen - Five Petals in At Five Petals Hotel & Banquets, Near Chanakyapuri Bridge, Ghatlodia, Ahmedabad rated 4.2 with avg cost 1200 \n\nYanki Sizzlers in 4, Ground Floor, Binori Ambit, Next to Renault Showroom, Thaltej Circle, Thaltej, Ahmedabad rated 4.1 with avg cost 1200 \n\nPatang - The Revolving Restaurant in Chinubhai Tower, Nehru Bridge Corner, Ashram Road, Ahmedabad rated 3.7 with avg cost 1800 \n\n"}
    - utter_email
* email_input{"email": "af.y@ymail.com"}
    - slot{"email": "af.y@ymail.com"}
    - action_send_mail
    - slot{"email": "af.y@ymail.com"}
    - utter_mail_confirmation
    - utter_goodbye
* affirm

* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "Ahmedabad"}
    - slot{"location": "Ahmedabad"}
    - slot{"location": "Ahmedabad"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - utter_ask_budget
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - action_search_restaurants
    - slot{"location": "Ahmedabad"}
    - slot{"response": "Lollo Rosso in Shop 2, Ground Floor, Aeon Complex, Opposite Navkar Institute, Navrangpura, Ahmedabad rated 4.6 with avg cost 1000 \n\nBrick Kitchen in At Five Petals Hotel & Banquets, Near Chanakyapuri Bridge, Ghatlodia, Ahmedabad rated 4.3 with avg cost 900 \n\n650 - The Global Kitchen in Shreekunj Mandapam, Beside Golden Tulip Bunglows & Tulip Citadel, Manekbaug, Ambavadi, Ahmedabad rated 4.2 with avg cost 900 \n\nBrick Kitchen - Five Petals in At Five Petals Hotel & Banquets, Near Chanakyapuri Bridge, Ghatlodia, Ahmedabad rated 4.2 with avg cost 1200 \n\nYanki Sizzlers in 4, Ground Floor, Binori Ambit, Next to Renault Showroom, Thaltej Circle, Thaltej, Ahmedabad rated 4.1 with avg cost 1200 \n\nPatang - The Revolving Restaurant in Chinubhai Tower, Nehru Bridge Corner, Ashram Road, Ahmedabad rated 3.7 with avg cost 1800 \n\n"}
    - utter_email
* email_input{"email": "af.y@ymail.com"}
    - slot{"email": "af.y@ymail.com"}
    - slot{"email": "af.y@ymail.com"}
    - action_send_mail
    - slot{"email": "af.y@ymail.com"}
    - utter_mail_confirmation
    - utter_goodbye
* restaurant_search{"budget": "More than 700", "cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - slot{"budget": "More than 700"}
    - utter_ask_location
* restaurant_search{"location": "amritsar"}
    - slot{"location": "amritsar"}
    - action_search_restaurants
    - slot{"location": "amritsar"}
    - slot{"response": "Sakhis Watz Kukin in M 47, Green Avenue, Opposite Main Park, Ranjit Avenue, Amritsar rated 4.3 with avg cost 800 \n\nThe Yellow Chilli in 108, GRD Towers, District Shopping Center, Ranjit Avenue, Amritsar rated 3.4 with avg cost 1200 \n\n"}
    - utter_email
* deny
    - utter_goodbye
* goodbye

* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "Ahmedabad"}
    - slot{"location": "Ahmedabad"}
    - slot{"location": "Ahmedabad"}
    - slot{"location": "Ahmedabad"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - utter_ask_budget
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - action_search_restaurants
    - slot{"location": "Ahmedabad"}
    - slot{"response": "Lollo Rosso in Shop 2, Ground Floor, Aeon Complex, Opposite Navkar Institute, Navrangpura, Ahmedabad rated 4.6 with avg cost 1000 \n\nBrick Kitchen in At Five Petals Hotel & Banquets, Near Chanakyapuri Bridge, Ghatlodia, Ahmedabad rated 4.3 with avg cost 900 \n\n650 - The Global Kitchen in Shreekunj Mandapam, Beside Golden Tulip Bunglows & Tulip Citadel, Manekbaug, Ambavadi, Ahmedabad rated 4.2 with avg cost 900 \n\nBrick Kitchen - Five Petals in At Five Petals Hotel & Banquets, Near Chanakyapuri Bridge, Ghatlodia, Ahmedabad rated 4.2 with avg cost 1200 \n\nYanki Sizzlers in 4, Ground Floor, Binori Ambit, Next to Renault Showroom, Thaltej Circle, Thaltej, Ahmedabad rated 4.1 with avg cost 1200 \n\nPatang - The Revolving Restaurant in Chinubhai Tower, Nehru Bridge Corner, Ashram Road, Ahmedabad rated 3.7 with avg cost 1800 \n\n"}
    - utter_email
* email_input{"email": "af.y@ymail.com"}
    - slot{"email": "af.y@ymail.com"}
    - slot{"email": "af.y@ymail.com"}
    - slot{"email": "af.y@ymail.com"}
    - action_send_mail
    - slot{"email": "af.y@ymail.com"}
    - utter_mail_confirmation
    - utter_goodbye
* restaurant_search{"budget": "More than 700", "cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - slot{"budget": "More than 700"}
    - slot{"cuisine": "chinese"}
    - slot{"budget": "More than 700"}
    - utter_ask_location
* restaurant_search{"location": "amritsar"}
    - slot{"location": "amritsar"}
    - slot{"location": "amritsar"}
    - action_search_restaurants
    - slot{"location": "amritsar"}
    - slot{"response": "Sakhis Watz Kukin in M 47, Green Avenue, Opposite Main Park, Ranjit Avenue, Amritsar rated 4.3 with avg cost 800 \n\nThe Yellow Chilli in 108, GRD Towers, District Shopping Center, Ranjit Avenue, Amritsar rated 3.4 with avg cost 1200 \n\n"}
    - utter_email
* deny
    - utter_goodbye
* restaurant_search{"cuisine": "mexican", "budget": "Lesser than 300"}
    - slot{"cuisine": "mexican"}
    - slot{"budget": "Lesser than 300"}
    - utter_ask_location
* restaurant_search{"location": "puducherry"}
    - slot{"location": "puducherry"}
    - action_search_restaurants
    - slot{"location": "puducherry"}
    - slot{"response": ""}
    - utter_goodbye

* greet
    - utter_greet
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - utter_ask_location
* restaurant_search{"location": "kanpur"}
    - slot{"location": "kanpur"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - action_search_restaurants
    - slot{"location": "kanpur"}
    - slot{"response": "Royal Dine - Hotel Royal Cliff in Hotel Royal Cliff, 113 / 72, Near Motijheel Garden, Swaroop Nagar, Kanpur rated 4.0 with avg cost 1500 \n\nChin Mi in Rave 3, Plot 11, Block 6 Parwati Bagla Road, Tilak Nagar, Kanpur rated 3.9 with avg cost 1500 \n\nWaterside - The Landmark Hotel in The Landmark Hotel, Landmark Towers, 10, Near Naveen Market, Mall Road, Kanpur rated 3.9 with avg cost 3000 \n\nVerandah in Third Floor, 7/17, Parvati Bagla Road, Tilak Nagar, Kanpur rated 3.7 with avg cost 1500 \n\nAnaicha's Food Joint in 113/187, Swaroop Nagar, Kanpur rated 3.6 with avg cost 850 \n\n"}
    - utter_email
* restaurant_search{"location": "mysore"}
    - slot{"location": "mysore"}
    - action_search_restaurants
    - slot{"location": "mysore"}
    - slot{"response": "Jalpaan Dining Saga in 366, 2nd And 3rd Floor, Near Ramaswamy Circle, Chamaraja Mohalla, Chamrajpura, Mysore rated 4.3 with avg cost 900 \n\nBig Chicken in 331/A, Loyal World Building, Adjacent To St Josephs Hospital, Bannimantap, Mysore rated 4.0 with avg cost 1000 \n\nGufha Restaurant in 35/A, Pai Hotels, Bangalore Nilgiri Road, Doora, Mysore rated 3.9 with avg cost 1000 \n\nJalpaan Dining Saga in 366, 2nd & 3rd Floor, Near Ramaswamy Circle, Chamaraja Mohalla, Chamrajpura, Mysore rated 3.7 with avg cost 900 \n\nJungle The Restaurant in Pai Hotels, Bangalore Nilgiri Road, Opposite Suburban Bus Stand, Mysore, Doora, Mysore rated 3.7 with avg cost 1000 \n\nThe Barge Restaurant in Plot 440A, Hebbal Industrial Area, Near Infosys Campus, Vijay Nagar, Mysore rated 3.3 with avg cost 1500 \n\n"}
    - utter_email
* deny
    - utter_goodbye
* affirm

* greet
    - utter_greet
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - utter_ask_location
* restaurant_search{"location": "kanpur"}
    - slot{"location": "kanpur"}
    - slot{"location": "kanpur"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - action_search_restaurants
    - slot{"location": "kanpur"}
    - slot{"response": "Royal Dine - Hotel Royal Cliff in Hotel Royal Cliff, 113 / 72, Near Motijheel Garden, Swaroop Nagar, Kanpur rated 4.0 with avg cost 1500 \n\nChin Mi in Rave 3, Plot 11, Block 6 Parwati Bagla Road, Tilak Nagar, Kanpur rated 3.9 with avg cost 1500 \n\nWaterside - The Landmark Hotel in The Landmark Hotel, Landmark Towers, 10, Near Naveen Market, Mall Road, Kanpur rated 3.9 with avg cost 3000 \n\nVerandah in Third Floor, 7/17, Parvati Bagla Road, Tilak Nagar, Kanpur rated 3.7 with avg cost 1500 \n\nAnaicha's Food Joint in 113/187, Swaroop Nagar, Kanpur rated 3.6 with avg cost 850 \n\n"}
    - utter_email
* restaurant_search{"location": "mysore"}
    - slot{"location": "mysore"}
    - slot{"location": "mysore"}
    - action_search_restaurants
    - slot{"location": "mysore"}
    - slot{"response": "Jalpaan Dining Saga in 366, 2nd And 3rd Floor, Near Ramaswamy Circle, Chamaraja Mohalla, Chamrajpura, Mysore rated 4.3 with avg cost 900 \n\nBig Chicken in 331/A, Loyal World Building, Adjacent To St Josephs Hospital, Bannimantap, Mysore rated 4.0 with avg cost 1000 \n\nGufha Restaurant in 35/A, Pai Hotels, Bangalore Nilgiri Road, Doora, Mysore rated 3.9 with avg cost 1000 \n\nJalpaan Dining Saga in 366, 2nd & 3rd Floor, Near Ramaswamy Circle, Chamaraja Mohalla, Chamrajpura, Mysore rated 3.7 with avg cost 900 \n\nJungle The Restaurant in Pai Hotels, Bangalore Nilgiri Road, Opposite Suburban Bus Stand, Mysore, Doora, Mysore rated 3.7 with avg cost 1000 \n\nThe Barge Restaurant in Plot 440A, Hebbal Industrial Area, Near Infosys Campus, Vijay Nagar, Mysore rated 3.3 with avg cost 1500 \n\n"}
    - utter_email
* deny
    - utter_goodbye
* restaurant_search{"location": "ludhiana"}
    - slot{"location": "ludhiana"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "Rs. 300 to 700"}
    - slot{"budget": "Rs. 300 to 700"}
    - action_search_restaurants
    - slot{"location": "ludhiana"}
    - slot{"response": "Basant in Fountain Chowk, Civil Lines, Ludhiana rated 4.4 with avg cost 500 \n\nRishi Vaishno Dhaba in 1185, Deep Nagar, Gill Road, Ludhiana rated 4.3 with avg cost 500 \n\nRishi Vegetarian Dhaba (RVN) in 9-11, Opposite Krishna Charitable Hospital, Model Town, Ludhiana rated 4.3 with avg cost 400 \n\nPandit Ji De Paranthe in SCO 30, Feroze Gandhi Market, Gurdev Nagar, Ludhiana rated 4.2 with avg cost 400 \n\nGopal Sweets in 1E, Malher Cinema Road, E-Block, Sarabha Nagar, Ludhiana rated 4.2 with avg cost 450 \n\nBasant in Fountain Chowk, Civil Lines, Ludhiana rated 3.9 with avg cost 400 \n\n"}
    - utter_email
* email_input{"email": "hey@by.com"}
    - slot{"email": "hey@by.com"}
    - action_send_mail
    - slot{"email": "hey@by.com"}
    - utter_mail_confirmation
    - utter_goodbye
* goodbye

* greet
    - utter_greet
* restaurant_search{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - slot{"budget": "More than 700"}
    - utter_ask_location
* restaurant_search{"location": "kanpur"}
    - slot{"location": "kanpur"}
    - slot{"location": "kanpur"}
    - slot{"location": "kanpur"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - action_search_restaurants
    - slot{"location": "kanpur"}
    - slot{"response": "Royal Dine - Hotel Royal Cliff in Hotel Royal Cliff, 113 / 72, Near Motijheel Garden, Swaroop Nagar, Kanpur rated 4.0 with avg cost 1500 \n\nChin Mi in Rave 3, Plot 11, Block 6 Parwati Bagla Road, Tilak Nagar, Kanpur rated 3.9 with avg cost 1500 \n\nWaterside - The Landmark Hotel in The Landmark Hotel, Landmark Towers, 10, Near Naveen Market, Mall Road, Kanpur rated 3.9 with avg cost 3000 \n\nVerandah in Third Floor, 7/17, Parvati Bagla Road, Tilak Nagar, Kanpur rated 3.7 with avg cost 1500 \n\nAnaicha's Food Joint in 113/187, Swaroop Nagar, Kanpur rated 3.6 with avg cost 850 \n\n"}
    - utter_email
* restaurant_search{"location": "mysore"}
    - slot{"location": "mysore"}
    - slot{"location": "mysore"}
    - slot{"location": "mysore"}
    - action_search_restaurants
    - slot{"location": "mysore"}
    - slot{"response": "Jalpaan Dining Saga in 366, 2nd And 3rd Floor, Near Ramaswamy Circle, Chamaraja Mohalla, Chamrajpura, Mysore rated 4.3 with avg cost 900 \n\nBig Chicken in 331/A, Loyal World Building, Adjacent To St Josephs Hospital, Bannimantap, Mysore rated 4.0 with avg cost 1000 \n\nGufha Restaurant in 35/A, Pai Hotels, Bangalore Nilgiri Road, Doora, Mysore rated 3.9 with avg cost 1000 \n\nJalpaan Dining Saga in 366, 2nd & 3rd Floor, Near Ramaswamy Circle, Chamaraja Mohalla, Chamrajpura, Mysore rated 3.7 with avg cost 900 \n\nJungle The Restaurant in Pai Hotels, Bangalore Nilgiri Road, Opposite Suburban Bus Stand, Mysore, Doora, Mysore rated 3.7 with avg cost 1000 \n\nThe Barge Restaurant in Plot 440A, Hebbal Industrial Area, Near Infosys Campus, Vijay Nagar, Mysore rated 3.3 with avg cost 1500 \n\n"}
    - utter_email
* deny
    - utter_goodbye
* restaurant_search{"location": "ludhiana"}
    - slot{"location": "ludhiana"}
    - slot{"location": "ludhiana"}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - utter_ask_budget
* restaurant_search{"budget": "Rs. 300 to 700"}
    - slot{"budget": "Rs. 300 to 700"}
    - slot{"budget": "Rs. 300 to 700"}
    - action_search_restaurants
    - slot{"location": "ludhiana"}
    - slot{"response": "Basant in Fountain Chowk, Civil Lines, Ludhiana rated 4.4 with avg cost 500 \n\nRishi Vaishno Dhaba in 1185, Deep Nagar, Gill Road, Ludhiana rated 4.3 with avg cost 500 \n\nRishi Vegetarian Dhaba (RVN) in 9-11, Opposite Krishna Charitable Hospital, Model Town, Ludhiana rated 4.3 with avg cost 400 \n\nPandit Ji De Paranthe in SCO 30, Feroze Gandhi Market, Gurdev Nagar, Ludhiana rated 4.2 with avg cost 400 \n\nGopal Sweets in 1E, Malher Cinema Road, E-Block, Sarabha Nagar, Ludhiana rated 4.2 with avg cost 450 \n\nBasant in Fountain Chowk, Civil Lines, Ludhiana rated 3.9 with avg cost 400 \n\n"}
    - utter_email
* email_input{"email": "hey@by.com"}
    - slot{"email": "hey@by.com"}
    - slot{"email": "hey@by.com"}
    - action_send_mail
    - slot{"email": "hey@by.com"}
    - utter_mail_confirmation
    - utter_goodbye
* restaurant_search{"cuisine": "asian fusion"}
    - slot{"cuisine": "asian fusion"}
    - utter_ask_budget
* restaurant_search{"budget": "Rs. 300 to 700"}
    - slot{"budget": "Rs. 300 to 700"}
    - utter_ask_location
* restaurant_search{"location": "surat"}
    - slot{"location": "surat"}
    - action_search_restaurants
    - utter_goodbye
