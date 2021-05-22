## intent:affirm
- yes
- yep
- yeah
- indeed
- that's right
- ok
- great
- right, thank you
- correct
- great choice
- sounds really good
- thanks
- thank you
- thanks a lot

## intent:deny
- no
- nope
- no, thanks!
- not required
- no need
- not interested
- i'm good
- that's all

## intent:goodbye
- bye
- goodbye
- good bye
- stop
- end
- farewell
- Bye bye
- have a good one

## intent:greet
- hey
- howdy
- hey there
- hello
- hi
- good morning
- good evening
- good afternoon
- good noon
- noon
- dear sir
- hola
- Hola
- Hello
- heyy
- hie

## intent:restaurant_search
- i'm looking for a place to eat
- I want to grab lunch
- I am searching for a dinner spot
- I am looking for a place to eat in [Nashik](location)
- I am hungry
- What's good in [Ahmedabad](location)?
- Suggest some good places for lunch in [Bangalore](location)
- Suggest some good places for dinner in [Mumbai](location)
- Show me what's good in [Gurgaon](location)
- Best restaurants in [Faridabad](location)
- Top five restaurants in [Bhubaneshwar](location)
- Top ten places to eat in [Ahemdabad]{"entity": "location", "value": "Ahmedabad"}
- Show me top 10 restaurants in [Dubai](location)
- Top 20 food joints in [America](location)
- I am looking for some restaurants in [Delhi](location).
- I am looking for some restaurants in [Bangalore](location)
- show me [chinese](cuisine) restaurants
- Suggest some good restaurant for [South Indian](location)
- show me [chines]{"entity": "cuisine", "value": "chinese"} restaurants in the [New Delhi]{"entity": "location", "value": "Delhi"}
- show me a [mexican](cuisine) place in the [Patna](location)
- Authentic [chinese](cuisine) places in [Delhi](location)
- i am looking for an [indian](cuisine) spot called olaolaolaolaolaola
- search for restaurants
- anywhere in the [west](location)
- I am looking for [asian fusion](cuisine) food
- I am looking for [street food](cuisine) food
- I am looking for a restaurant in [294328](location)
- in [Gurgaon](location)
- [South Indian](cuisine)
- [North Indian](cuisine)
- [Italian](cuisine)
- [American](cuisine)
- [Chinese]{"entity": "cuisine", "value": "chinese"}
- [chinese](cuisine)
- [Lithuania](location)
- Oh, sorry, in [Mysore](location)
- in [delhi](location)
- I am looking for some restaurants in [Mumbai](location)
- I am looking for [mexican indian fusion](cuisine)
- I want [exotic]{"entity": "budget", "value": "More than 700"} [mexican](cuisine) food.
- can you book a table in [Aurangabad](location) in a [moderate]{"entity": "budget", "value": "Rs. 300 to 700"} price range with [british](cuisine) food for four people
- I want to eat [cheap]{"entity": "budget", "value": "Lesser than 300"} [chinese](cuisine) food
- I want to eat [expensive]{"entity": "budget", "value": "More than 700"} [Italian](cuisine) food in [Mumbai](location)
- [central](location) [indian](cuisine) restaurant
- please help me to find restaurants in [pune](location)
- Please find me a restaurant in [bangalore](location)
- Please find me [cheap]{"entity": "budget", "value": "Lesser than 300"} restaurants in [Mangalore](location)
- I want to eat in a [pocket friendly]{"entity": "budget", "value": "Lesser than 300"} restaurant
- I am looking for [budget friendly]{"entity": "budget", "value": "Lesser than 300"} [South Indian](cuisine) restaurants
- I would like to eat [North-Indian]{"entity": "cuisine", "value": "North Indian"} cuisine in an [average]{"entity": "budget", "value": "Rs. 300 to 700"} priced hotel
- We want [mexican](cuisine) food which is [expensive]{"entity": "budget", "value": "More than 700"}
- Suggest me some [expensive]{"entity": "budget", "value": "More than 700"} hotels for food
- I am looking for a [inexpensive]{"entity": "budget", "value": "Lesser than 300"} theme restaurant in [Puducherry](location)
- [mumbai](location)
- show me restaurants
- Find restaurants
- please find me [chinese](cuisine) restaurant in [delhi](location)
- can you find me a [chinese](cuisine) restaurant
- [delhi](location)
- please find me a restaurant in [ahmedabad](location)
- please show me a few [italian](cuisine) restaurants in [bangalore](location)
- I want food
- [egypt](location)
- [delhi](location) [mexican](cuisine)
- [american](cuisine)
- [gurgaon](location)
- [amritsar](location)
- [burmese](cuisine)
- [nasik]{"entity": "location", "value": "Nashik"}
- [Mexican](cuisine)
- where can i find good food?
- [Faridabad](location)
- I'm hungry. Looking out for some good restaurants
- [Malegaon](location)
- [Lesser than 300](budget)
- [Rs. 300 to 700](budget)
- [More than 700](budget)
- i'm hungry, looking for food
- [chandigarh](location)
- hungry
- I'm hungry. looking out for some good [chinese](cuisine) restaurants in [Chandigarh](location)
- [cheap]{"entity": "budget", "value": "Lesser than 300"} [chinese](cuisine) restaurant in [gurgaon](location)
- [expensive]{"entity": "budget", "value": "More than 700"} [italian](cuisine) hotel in [mumbai](location)

## intent:email_input
- [abcd_123@gmail.com](email)
- My email id is [randomyguy@yahoo.com](email)
- Email : [rahul@outlook.com](email)
- [hello@ymail.com](email)
- [test@outlook.com](email)
- [abd@dev.com](email)
- [test@gmail.com](email)

## synonym: Mumbai
- Bombay

## synonym:Ahmedabad
- Ahemdabad

## synonym:Chennai
- Madras

## synonym:Delhi
- New Delhi
- Dilli
- Old Delhi
- New-Delhi
- Old-Delhi

## synonym:Gurgaon
- Gurugram

## synonym:Lesser than 300
- cheap
- pocket friendly
- budget friendly
- inexpensive
- nominal
- economic

## synonym:More than 700
- exotic
- expensive
- costly

## synonym:Mysore
- Mysuru

## synonym:Nashik
- nasik
- Nasik

## synonym:North Indian
- North-Indian

## synonym:Puducherry
- Pondicherry

## synonym:Rs. 300 to 700
- moderate
- average

## synonym:South Indian
- South-Indian

## synonym:bangalore
- Bengaluru

## synonym:chinese
- chines
- Chinese
- Chines

## synonym:vegetarian
- veggie
- vegg

## regex:email
- ^[a-z_.0-9]{4,20}@[a-z]{3,15}\.(com|in|org)$

## regex:greet
- hey[^\s]\*
