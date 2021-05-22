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
- I want [exotic]{"entity": "price", "value": "high"} [mexican](cuisine) food.
- can you book a table in [Aurangabad](location) in a [moderate]{"entity": "price", "value": "mid"} price range with [british](cuisine) food for four people
- I want to eat [cheap]{"entity": "price", "value": "low"} [chinese](cuisine) food
- I want to eat [expensive]{"entity": "price", "value": "high"} [Italian](cuisine) food in [Mumbai](location)
- [central](location) [indian](cuisine) restaurant
- please help me to find restaurants in [pune](location)
- Please find me a restaurant in [bangalore](location)
- Please find me [cheap]{"entity": "price", "value": "low"} restaurants in [Mangalore](location)
- I want to eat in a [pocket friendly]{"entity": "price", "value": "low"} restaurant
- I am looking for [budget friendly]{"entity": "price", "value": "low"} [South Indian](cuisine) restaurants
- I would like to eat [North-Indian]{"entity": "cuisine", "value": "North Indian"} cuisine in an [average]{"entity": "price", "value": "mid"} priced hotel
- We want [mexican](cuisine) food which is [expensive]{"entity": "price", "value": "high"}
- Suggest me some [expensive]{"entity": "price", "value": "high"} hotels for food
- I am looking for a [inexpensive]{"entity": "price", "value": "low"} theme restaurant in [Puducherry](location)
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
- [Italian](cuisine)

## intent:email_input
- [abcd_123@gmail.com](email)
- My email id is [randomyguy@yahoo.com](email)
- Email : [rahul@outlook.com](email)
- [hello@ymail.com](email)
- [test@outlook.com](email)

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

## synonym:Mysore
- Mysuru

## synonym:Nashik
- nasik
- Nasik

## synonym:Puducherry
- Pondicherry

## synonym:South Indian
- North-Indian
- South-Indian

## synonym:bangalore
- Bengaluru

## synonym:chinese
- chines
- Chinese
- Chines

## synonym:high
- exotic
- expensive
- costly

## synonym:low
- cheap
- pocket friendly
- budget friendly
- inexpensive
- nominal
- economic

## synonym:mid
- moderate
- average

## synonym:vegetarian
- veggie
- vegg

## regex:email
- ^[a-z_.0-9]{4,20}@[a-z]{3,15}\.(com|in|org)$

## regex:greet
- hey[^\s]\*

## regex:pincode
- [0-9]{6}
