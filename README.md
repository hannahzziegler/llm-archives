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

This is pretty impressive. I like that the list of people, places and organizations mentioned in the CNS and Diamondback stories are itemized and in a structured format. It would be really helpful for The Diamondback to have a story archive that can be queried in this way, especially in terms of analyzing which sources we rely most heavily on over time. If we pulled all of this information for the news stories across the last 5-10 years, we'd have a pretty robust source list of folks we've spoken to in the past. I would want to build up structured data from each Diamondback story to maintain a spreadsheet of who we've spoken to and when. The feature that clocks when various organizations are mentioned in the text would also be helpful in doing a source and organization-wide audit of how often we speak to different communities on campus, especially the groups that target those from underrepresented backgrounds such as Black Student Union, Asian American Student Union and so on. By maintaining these records, The Diamondback would be able to complete internal coverage audits easier and make sure its reporters are reaching out to as many sources as possible. 