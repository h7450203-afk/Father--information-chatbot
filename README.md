print("===== Father Information Chatbot =====")
print("Type 'exit' to quit.\n")

# Extended Dictionary with old job and extra details (Village removed)
father = {
    "name": "Adrees",
    "age": "62 years",
    "work": "Senior Khatib at Mudrisa Anwarul Alooom",
    "education": "Hifzul Quran",
    "problem": "Training teachers and students and visiting branches for tests",
    "old job": "Farmer (Agriculture background)",
    "hobby": "Reading Islamic books and gardening",
    "residence": "Multan, Punjab, Pakistan"
}

# Main loop for continuous interaction
while True:
    # Taking user input and converting to lowercase for normalization
    user_input = input("You: ").lower()
    
    # Check for exit command
    if user_input == "exit":
        print("Bot: Thank you! Goodbye.")
        # Breaking the loop to close the program
        break
        
    # Checking for keywords using 'in' operator
    elif "name" in user_input:
        print("Bot:", father["name"])
        
    elif "age" in user_input:
        print("Bot:", father["age"])
        
    elif "current work" in user_input or "job" in user_input or "profession" in user_input:
        print("Bot:", father["work"])
        
    elif "education" in user_input or "qualification" in user_input:
        print("Bot:", father["education"])
        
    elif "problem" in user_input or "challenge" in user_input:
        print("Bot:", father["problem"])
        
    elif "old job" in user_input or "farmer" in user_input or "past work" in user_input:
        print("Bot:", father["old job"])
        
    elif "hobby" in user_input or "free time" in user_input:
        print("Bot:", father["hobby"])
        
    elif "live" in user_input or "residence" in user_input:
        print("Bot:", father["residence"])
        
    # Default response for unknown queries
    else:
        print("Bot: Sorry, I don't have information about that. Please ask about his name, age, work, old job, etc.")
