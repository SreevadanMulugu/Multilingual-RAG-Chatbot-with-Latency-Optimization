# Multilingual-RAG-Chatbot-with-Latency-Optimization

<br>

🤖 AI Chatbot for Generic Money Website FAQs

Flowdiagram
<img width="2257" height="2068" alt="Untitled diagram-2025-10-08-135448" src="https://github.com/user-attachments/assets/8dbf77a4-828a-41d7-85d4-e3bca9767a3e" />

<br>
<br>

Hey there\! This is a cool project that builds a smart chatbot. Its main job is to answer questions people might have about Generic Money, a digital bank.

<br>

Think of it as an AI assistant that has read all of the Frequently Asked Questions (FAQs) on the Generic website and is ready to help users. The best part? It can chat in any language and is super fast for common questions.

<br>
<br>
<br>

✨ **What Makes This Chatbot Special?**

<br>

This isn't just a simple bot. It has two really neat features:

<br>

  * **It Speaks Your Language:** You can ask a question in English, Hinglish, Telugu, or any other language you want. The bot will understand it, find the answer, and reply to you in the same language you used.

<br>

  * **It's Super Fast for Easy Questions:** If you ask something that is very similar to a question already on the Generic FAQ page, the bot takes a shortcut. It finds that question and gives you the answer right away, skipping the need to think with its big AI brain. This makes it really quick\! For new or tricky questions, it uses its powerful AI to figure out the best response.

<br>
<br>
<br>

⚙️ **How Does It Work? A Simple Breakdown**

<br>

The whole project works in a few steps, all written in a single Jupyter Notebook.

<br>

  * **Get the Information:** First, the program acts like a mini-robot and visits the Generic Money "Contact Us" page. It reads and copies all the questions and answers from the FAQ section. This is called web scraping.

<br>

  * **Clean Up the Text:** The copied text can be a bit messy. This step cleans everything up, removing extra spaces or code, to make it easy for the AI to read.

<br>

  * **Create a Smart Library (FAISS Index):** The bot needs a way to quickly search through all the FAQs. It turns every question into a special code (called an "embedding"). Then, it organizes all these codes in a super-efficient digital library called FAISS. This lets it find the most similar question in a fraction of a second.

<br>

  * **The Brain of the Operation (The LLM):** The project uses a powerful AI model from Microsoft called Phi-4-mini-instruct. This is the "brain" that can understand questions and write human-like answers.

<br>

  * **Answering a Question:** When you ask something:
      * The bot first checks if your question is a close match to one in its FAISS library.
      * **If it's a close match:** It shows you the answer directly (this is the fast shortcut\!).
      * **If it's a new question:** It finds a few related FAQs from its library to use as context. It sends your question and this context to the AI brain (the LLM). The brain then writes a helpful, custom answer for you.

<br>
<br>
<br>

🚀 **How to Run This Project**

<br>

You can run this entire project in Google Colab, which gives you a powerful computer for free.

<br>

  * **Open the Notebook:** Upload and open the `AI_Intern (2).ipynb` file in Google Colab.

<br>

  * **Turn on the GPU:** To make the AI run faster, go to `Runtime > Change runtime type` and select `T4 GPU` from the hardware accelerator dropdown.

<br>

  * **Run the Cells:** Just run each block of code (called a cell) from the top to the bottom.

<br>

  * The first cell will install all the necessary tools.

<br>

  * The next few cells will do the scraping, cleaning, and setup.

<br>

  * The final cell will start a simple chat interface right there in the notebook.

<br>

  * **Start Chatting\!** Once you see the prompt `You:`, you can type your question and press Enter. Type `quit` when you want to stop.

<br>
<br>
<br>

That's it\! You've built and are now running a powerful, multilingual AI chatbot.


