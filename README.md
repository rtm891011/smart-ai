
## Smart AI
I created a ai that can answer questions on physics and a few other sciences
## The Algorithm
This AI is a chatbot spefically designed for physics and other sciences i gave it multiple pages on chemistry, nuclear physics, rocket science, engineering photons, electro magentism and plasma phyisics.
## Running this project
for recreating this project use these sources in ollama for knowledge these are the links i used
https://en.wikipedia.org/wiki/Quantum_mechanics
https://en.wikipedia.org/wiki/Antimatter
https://en.wikipedia.org/wiki/Chemistry
https://en.wikipedia.org/wiki/Nuclear_physics
https://en.wikipedia.org/wiki/Engineering
https://en.wikipedia.org/wiki/Photon
https://en.wikipedia.org/wiki/Electromagnetism
https://en.wikipedia.org/wiki/Outline_of_physics
https://en.wikipedia.org/wiki/Plasma_(physics)

## how to set it up
Ollama is a Large Language Model (LLM) chatbot. It works similarly to ChatGPT. You can ask it questions and it will give you answers. You might ask what's impressive about running Ollama on the Orin vs Chat GPT?
Remember, AI isn't always correct and will often make things up.

Always give AI information a look to ensure it's accuracy..

Even though this AI is only partially correct, you'll learn how to create your own knowledge base to develop a chatbot that's knowledgeable in a topic of your choosing.

1. SSH into your Orin.

2. sudo docker run -d --network=host \
    -v ${HOME}/open-webui:/app/backend/data \
    -e OLLAMA_BASE_URL=http://127.0.0.1:11434 \
    --name open-webui \
    ghcr.io/open-webui/open-webui:main

3. Run and install Ollama.

    jetson-containers run --name ollama $(autotag ollama)

Once it finishes, you'll be in the Docker and Ollama will be running.

    ollama run llama3
This process will take a while.

Once it's done, you'll see success as below and be prompted to add some text.

4.  Talk to Ollama. Send it a message and it should reply.


You can stop Ollama by using Ctrl + D or /bye, and that will exit it. You'll need to use Ctrl + D once more to exit the Docker container as well.


Once you have Ollama running, you can connect to it in your browser.

1
Open a web browser.

2
Add  http://<JETSON-IP>:8080  to the address bar.

3
Replace <JETSON-IP>  with the IP address you use for SSH.

4
Press Enter to navigate to the URL.

5
If you see a security warning, ignore it and click Continue to site.

Once you're loaded in, you should see a big webpage with changing text and Get Started towards the bottom of the webpage.

6
Select Get Started to continue.

7
Enter a name, email, and password, then click Create Admin Account.

This page will ask you to log in. The account you create is only stored locally.

You can put in whatever you want to. You'll create new credentials when you reconnect. This information won't be saved anywhere but locally, so it isn't a security concern.
