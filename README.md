# AI-MED Web interface: A User-Friendly Web Interface for Chat Interactions 👋

![GitHub stars](https://img.shields.io/github/stars/ollama-webui/ollama-webui?style=social)
![GitHub forks](https://img.shields.io/github/forks/ollama-webui/ollama-webui?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/ollama-webui/ollama-webui?style=social)
![GitHub repo size](https://img.shields.io/github/repo-size/ollama-webui/ollama-webui)
![GitHub language count](https://img.shields.io/github/languages/count/ollama-webui/ollama-webui)
![GitHub top language](https://img.shields.io/github/languages/top/ollama-webui/ollama-webui)
![GitHub last commit](https://img.shields.io/github/last-commit/ollama-webui/ollama-webui?color=red)
![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Follama-webui%2Follama-wbui&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)
[![Discord](https://img.shields.io/badge/Discord-Ollama_Web_UI-blue?logo=discord&logoColor=white)](https://discord.gg/5rJgQTnV4s)
[![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/tjbck)

ChatGPT-Style Web Interface for Ayonix AI-MED 🦙

**Disclaimer:** Ayonix AI-MED is a commercial medial diagnostics utility and is not affiliated with the chatgpt or OpenAI in any way. This initiative is independent, and any inquiries or feedback should be directed to ayonix.com. We kindly request users to refrain from contacting or harassing the OPENAI regarding this project._

![Ollama Web UI Demo](./demo.gif)


## Features ⭐

- 🖥️ **Intuitive Interface**: Our chat interface takes inspiration from ChatGPT, ensuring a user-friendly experience.

- 📱 **Responsive Design**: Enjoy a seamless experience on both desktop and mobile devices.

- ⚡ **Swift Responsiveness**: Enjoy fast and responsive performance.

- ✒️🔢 **Full Markdown and LaTeX Support**: Elevate your experience with comprehensive Markdown and LaTeX capabilities for enriched interaction.

- 📚 **Local RAG Integration**: Dive into the future of chat interactions with the groundbreaking Retrieval Augmented Generation (RAG) support. This feature seamlessly integrates document interactions into your chat experience. You can load documents directly into the chat or add files to your document library, effortlessly accessing them using `#` command in the prompt. In its alpha phase, occasional issues may arise as we actively refine and enhance this feature to ensure optimal performance and reliability.

- 🌐 **Web Browsing Capability**: Seamlessly integrate websites into your chat experience using the `#` command followed by the URL. This feature allows you to incorporate web content directly into your conversations, enhancing the richness and depth of your interactions.

- 📜 **Prompt Preset Support**: Instantly access preset prompts using the `/` command in the chat input. Load predefined conversation starters effortlessly and expedite your interactions.
- 
- 👍👎 **RLHF Annotation**: Empower your messages by rating them with thumbs up and thumbs down, facilitating the creation of datasets for Reinforcement Learning from Human Feedback (RLHF). Utilize your messages to train or fine-tune models, all while ensuring the confidentiality of locally saved data.

- 🏷️ **Conversation Tagging**: Effortlessly categorize and locate specific chats for quick reference and streamlined data collection.

- 📥🗑️ **Download/Delete Models**: Easily download or remove models directly from the AI-MED web utility.

- ⬆️ **GGUF File Model Creation**: Effortlessly create Ayonix LLM models by uploading GGUF files directly from the web interface. Streamlined process with options to upload from your machine or download GGUF files from Ayonix website

- 🤖 **Multiple Model Support**: Seamlessly switch between different chat models for diverse interactions.

- 🔄 **Multi-Modal Support**: Seamlessly engage with models that support multimodal interactions, including images (e.g., LLava).

- ⚙️ **Many Models Conversations**: Effortlessly engage with various models simultaneously, harnessing their unique strengths for optimal responses. Enhance your experience by leveraging a diverse set of models in parallel.

- 💬 **Collaborative Chat**: Harness the collective intelligence of multiple models by seamlessly orchestrating group conversations. Use the `@` command to specify the model, enabling dynamic and diverse dialogues within your chat interface. Immerse yourself in the collective intelligence woven into your chat environment.

- 🤝 **OpenAI API Integration**: Effortlessly integrate OpenAI-compatible API for versatile conversations alongside Ayonix LLM Medical models. Customize the API Base URL to link with **LMStudio, Mistral, OpenRouter, and more**.

- 🔄 **Regeneration History Access**: Easily revisit and explore your entire regeneration history.

- 📜 **Chat History**: Effortlessly access and manage your conversation history.

- 📤📥 **Import/Export Chat History**: Seamlessly move your chat data in and out of the platform.

- 🗣️ **Voice Input Support**: Engage with your model through voice interactions; enjoy the convenience of talking to your model directly. Additionally, explore the option for sending voice input automatically after 3 seconds of silence for a streamlined experience.

- ⚙️ **Fine-Tuned Control with Advanced Parameters**: Gain a deeper level of control by adjusting parameters such as temperature and defining your system prompts to tailor the conversation to your specific preferences and needs.

- 🔗 **External AI-MED Server Connection**: Seamlessly link to an external Ollama server hosted on a different address by configuring the environment variable.

- 🔐 **Role-Based Access Control (RBAC)**: Ensure secure access with restricted permissions; only authorized individuals can access AI-MED, and exclusive model creation/pulling rights are reserved for administrators.

- 🔒 **Backend Reverse Proxy Support**: Bolster security through direct communication between Ayonix AI-MED Web backend and AI-MED Engine. This key feature eliminates the need to expose AI-MED over LAN. Requests made to the '/AI-MED/api' route from the web UI are seamlessly redirected to AI-MED from the backend, enhancing overall system security.

- 🌟 **Continuous Updates**: We are committed to improving Ayonix AI-MED Web interface with regular updates and new features.

## How to Install 🚀

🌟 **Important Note on User Roles and Privacy:**

- **Admin Creation:** The very first account to sign up on the Ayonix AI-MED Web will be granted **Administrator privileges**. This account will have comprehensive control over the platform, including user management and system settings.

- **User Registrations:** All subsequent users signing up will initially have their accounts set to **Pending** status by default. These accounts will require approval from the Administrator to gain access to the platform functionalities.

- **Privacy and Data Security:** We prioritize your privacy and data security above all. Please be reassured that all data entered into the AI-MED Web I/F is stored locally on your device. Our system is designed to be privacy-first, ensuring that no external requests are made, and your data does not leave your local environment. We are committed to maintaining the highest standards of data privacy and security, ensuring that your information remains confidential and under your control.


## What's Next? 🚀

### Roadmap 📝

Here are some exciting tasks on our roadmap:

- 🔊 **Local Text-to-Speech Integration**: Seamlessly incorporate text-to-speech functionality directly within the platform, allowing for a smoother and more immersive user experience.
- 🛡️ **Granular Permissions and User Groups**: Empower administrators to finely control access levels and group users according to their roles and responsibilities. This feature ensures robust security measures and streamlined management of user privileges, enhancing overall platform functionality.
- 🔄 **Function Calling**: Empower your interactions by running code directly within the chat. Execute functions and commands effortlessly, enhancing the functionality of your conversations.
- 🔧 **Fine-tune Model (LoRA)**: Fine-tune your model directly from the user interface. This feature allows for precise customization and optimization of the chat experience to better suit your needs and preferences.
- 🧠 **Long-Term Memory**: Witness the power of persistent memory in our agents. Enjoy conversations that feel continuous as agents remember and reference past interactions, creating a more cohesive and personalized user experience.
- 🧪 **Research-Centric Features**: Empower researchers in the fields of LLM and HCI with a comprehensive web UI for conducting user studies. Stay tuned for ongoing feature enhancements (e.g., surveys, analytics, and participant tracking) to facilitate their research.
- 📈 **User Study Tools**: Providing specialized tools, like heat maps and behavior tracking modules, to empower researchers in capturing and analyzing user behavior patterns with precision and accuracy.
- 📚 **Enhanced Documentation**: Elevate your setup and customization experience with improved, comprehensive documentation.

Feel free to contribute and help us make AI-MED even better! 🙌

### Platinum Sponsors 🤍

- We're looking for Sponsors and Investors
  You can donate to AI-MED and contribute our world:
  https://gofund.me/9b077db0
  
