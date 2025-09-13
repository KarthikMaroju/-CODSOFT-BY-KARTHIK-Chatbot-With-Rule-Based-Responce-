# -CODSOFT-BY-KARTHIK-Chatbot-With-Rule-Based-Responce-
This project focuses on developing a Rule-Based Chatbot that can interact with users by identifying queries and providing predefined responses. The chatbot uses simple if-else statements or pattern-matching techniques to simulate conversation flow.
# Rule-Based Chatbot in Python

def chatbot_response(user_input):
    user_input = user_input.lower()

    # Predefined rules (customized)
    rules = {
        "hi": "Hello! How can I help you?",
        "hello": "Hi there! What can I do for you?",
        "hii": "Hey! Nice to see you.",
        "where are you from": "I am from Vizianagaram.",
        "who are you": "I am Karthik, AI assistant.",
        "how are you": "I am fine, thanks for asking! How are you?",
        "what is your name": "I am a Rule-Based Chatbot created in Python.",
        "bye": "Goodbye! Have a nice day.",
        "thanks": "You're welcome! Happy to help."
    }

    # Check for matching rule
    if user_input in rules:
        return rules[user_input]
    else:
        return "Sorry Dude🙂, this bot responding some tasks only " 

# Main loop
print("🤖 Chatbot is running... (type 'bye' to exit)\n")
while True:
    user_text = input("You: ")
    response = chatbot_response(user_text)
    print("Bot:", response)
    if user_text.lower() == "bye":
        break
