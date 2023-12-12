- 👋 Hi, I’m @TheWrightNomad
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

import hashlib
username = "TheWrightNomad"
interests = "Your interests here"
learning = "What you're currently learning"
collaboration = "Type of projects you are interested in"
contact_info = "Your contact information or preferred communication channels"

message = f"""
- 👋 Hi, I’m @{hashlib.sha256(username.encode()).hexdigest()}
- 👀 I’m interested in {hashlib.sha256(interests.encode()).hexdigest()}
- 🌱 I’m currently learning {hashlib.sha256(learning.encode()).hexdigest()}
- 💞️ I’m looking to collaborate on {hashlib.sha256(collaboration.encode()).hexdigest()}
- 📫 How to reach me {hashlib.sha256(contact_info.encode()).hexdigest()}
"""

# Display the hidden message
print("Hidden Message:")
print(message)
