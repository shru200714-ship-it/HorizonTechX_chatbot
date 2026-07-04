# HorizonTechX_chatbot
# ==========================================
#           BASIC RULE-BASED CHATBOT
# ==========================================

def chatbot_response(user_input):
    """
    Returns the chatbot's response based on the user's input.
    """

    user_input = user_input.lower().strip()

    if user_input == "hello":
        return "Hello! Nice to meet you."

    elif user_input == "hi":
        return "Hi! How can I help you today?"

    elif user_input == "hey":
        return "Hey! Hope you're having a great day."

    elif user_input == "how are you":
        return "I'm doing great! Thanks for asking."

    elif user_input == "what is your name":
        return "I'm a simple Python Chatbot."

    elif user_input == "who created you":
        return "I was created using Python as a rule-based chatbot."

    elif user_input == "what can you do":
        return "I can answer simple predefined questions and have a basic conversation."

    elif user_input == "thank you":
        return "You're welcome!"

    elif user_input == "thanks":
        return "Happy to help!"

    elif user_input == "good morning":
        return "Good Morning! Have a wonderful day."

    elif user_input == "good afternoon":
        return "Good Afternoon!"

    elif user_input == "good evening":
        return "Good Evening!"

    elif user_input == "bye":
        return "Goodbye! Have a nice day."

    else:
        return "Sorry, I don't understand that. Please try another question."


def main():

    print("=" * 50)
    print("        WELCOME TO BASIC CHATBOT")
    print("=" * 50)

    print("\nYou can ask me things like:")
    print("- hello")
    print("- hi")
    print("- how are you")
    print("- what is your name")
    print("- who created you")
    print("- what can you do")
    print("- thank you")
    print("- bye\n")

    while True:

        user = input("You : ")

        response = chatbot_response(user)

        print("Bot :", response)

        if user.lower().strip() == "bye":
            break


# Program starts here
if __name__ == "__main__":
    main()
