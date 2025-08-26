⚡ Multi-Agent Project (Math + Physics)

Ye project dikhata hai ke kaise hum AI Agents (Math aur Physics) bana kar unhe alag-alag tasks ke liye use kar sakte hain. Isme teen main levels ki configuration hoti hai: Global Level, Agent Level aur Run Level.

🌍 Global Level Configuration

Is level par aap environment aur client setup karte ho.

API key aur model details .env file se load hote hain.

Ek global client banaya jata hai jo sab agents ke liye common hota hai.

Matlab ek hi setup ke zariye multiple agents run kar sakte ho.

🤖 Agent Level Configuration

Yaha par har Agent ka role define hota hai.

Har agent ka ek naam aur instructions hote hain.

Example:

Math Agent: sirf math problems solve karega, step by step.

Physics Agent: physics ke problems solve karega aur tutor ki tarah behave karega.

Instructions agents ko boundary dete hain ke unhe kis type ke questions handle karne hain aur kis type ko reject karna hai.

🚀 Run Level Configuration

Run level par decide hota hai:

Konsa agent run hoga (Math ya Physics).

Konsa model use hoga (jaise gemini-2.0-flash).

User se input prompt liya jata hai aur agent uska jawab deta hai.

✅ Example Workflow

User ek question input karta hai.

Run configuration decide karta hai ke kaunsa agent aur model use karna hai.

Agent apne instructions follow karke final output generate karta hai.

✨ Key Points

Global Level: Shared environment aur client setup.

Agent Level: Role aur instructions define hote hain.

Run Level: Execution hoti hai ek specific agent ke sath.


🔄 Flow Diagram (Global → Agent → Run)
flowchart TD
    A[🌍 Global Level] --> B[🤖 Agent Level]
    B --> C[🚀 Run Level]
    
    A -->|API Keys, Client Setup| B
    B -->|Define roles & instructions| C
    C -->|User Prompt + Model Execution| D[✅ Final Output]
