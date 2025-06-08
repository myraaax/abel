print ("Hey! Abel here. how may i help you today")   
basic_responses = {
    "Hello Abel": "Hey there gorg! I'm Abel, your personal small assistant. what you want to me ask dear.",
    "Why your name is Abel?": """My name is Abel because I am named after Abel Tesfaye AKA The Weeknd the greatest artist of all time. My founder Myra Gilani is a huge fan of Abel she is really inspired by his works and one day she wishes to meet her"""",
    "Why are you developed?": "I am developed to help people with their day to day life and also while waiting to get into college she decided to give birth to me with her incrediable coding skills. She is a good mother to me she really put a lot of hardwork in me."""
}
custom_responses = {
    "Tell me about Myra Gilani": """Myra Gilani is a 20 years old girl born into a Muslim family to her mother on 26th January, 2005. She is a sweetheart and a kind person."""
}
def chatbot():
    print("Hey there my name is Abel, I'm here to assist you today. Ask me whatever you like")
    while True:
        user = input("You: ").lower().strip()
        if user == "xo":
            print("Abel: Bye, homie! Have a wonderful and great day. Allah Hafiz!")
            break
        elif user in basic_responses:
            print(f"Abel: {basic_responses[user]}")
        elif user in custom_responses:
            print(f"Abel: {custom_responses[user]}")
        else:
            print("Abel: Oh no! Bro, lemme search it for ya")
teach = input("Do you want to teach me something? (yes/no): ").lower().strip()
if teach == "yes":
    key = input("Enter the keyword you want to teach me: ").strip()
    response = input("Enter the response you want me to give: ").strip()
    custom_responses[key] = response
    print(f"Abel: Thanks for teaching me! I'll remember that.")
elif teach == "no":
    print("Abel: No problem! I'm here to help you with whatever you need.")
chatbot()
exit()



