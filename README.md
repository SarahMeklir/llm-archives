# llm-archives

### Instructions

Click the "Use this template" button for this repository and choose "Create a new repository". You can give it the same name (llm-archives).

Once it's ready, go to [Groq](https://console.groq.com/keys) and follow the directions to get an API key. You'll need to login (or create an account if you don't have one).

Copy the API key value and then click on the Settings of your GitHub repository and click on "Secrets and variables" on the left side, then choose "Codespaces"

Click the green "New Repository Secret" button and paste your API Key into the "Secret" box, then put GROQ_API_KEY in the Name box above it. Click "Add Secret" and click on the name of the repository to return to the main page.

From there, click the green "Code" button and create a new Codespace in the Codespaces tab.

In the Terminal type the following: pip install requests groq and hit enter.

Then type: python get_stories.py

You should see a file called cns_maryland_posts.json appear. Let's look at it. It contains some details of the past 10 CNS stories.

Back in the Terminal, type: python entity_extraction.py and watch the output.

### Evaluation for JOUR389W

It did very well! I don't see any errors, and the information it pulled was all relevant and important to the story. The story I chose had few individuals involved, but it pulled the name of the main subject of the story, the person interviewed, the writer, and the credited photographer. If the Banner had a collection of these across its archives, it would be able to use it as data to study and analyze. They could track the names featuring most commonly in their stories. They could easily see how many times they've asked one source for comment, and whether they need to diversify the voices in their stories. They could look at what locations their stories involve, and study patterns about why certain people or organizations are tied to each other. Also, since the data includes a description of each person, if a journalist was looking for a source who's an expert in a certain field, they could search this much more manageable story archive to find sources used in the past.