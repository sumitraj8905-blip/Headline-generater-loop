# Headline-generater-loop

#1-import the random module
import random
#create subjects
subjects =[
    "Shahrukh khan",
    "Virat kohli",
    "MS dhoni",
    "A Mumbai Cat",
    "A Group of Monkeys",
    "Prime Minister Modi"
]

actions =[
    "launches",
    "cancel",
    "dance with",
    "eats",
    "order",
    "celebrate",
]

places_or_things =[
    "at Red Fort",
    "in Mumbai Local Train",
    "a plate of samosa",
    "inside parliament",
    "during IPL match",
    "at Ganga ghat",
]

#3 start headline generation loop
while True:
    subject = random.choice(subjects)
    action = random.choice(actions)
    place_or_thing = random.choice(places_or_things)

    headline = f" BREAKING NEWS: {subject} {action} {place_or_thing}"
    print("\n" + headline)

    user_input = input("\nDo you want another headline? (yes/no)").strip().lower()
    if user_input == "no":
        break

    #print goodbye message
    print("\nThanks for using the Fake News Healdine Generator. Have a fun day")
