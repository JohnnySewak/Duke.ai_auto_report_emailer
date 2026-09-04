# Duke.ai automatic report emailer

An unpaid internship project for Duke.ai which:

1. Loops through user ids and emails from a excel spreadsheet in the same folder and with each set of user ids and emails does steps 2-5
2. Queries the Duke.ai API to generate an expenses breakdown on the given company using the user id from the aforementioned spreadsheet using the API POST command
3. Downloads the expenses pdf breakdown from the Duke.ai API using the API GET command
4. Sends the raw text from said pdf to ChatGPT to generate an email report in html
5. Uses the python library yagmail through a 2FA enabled Gmail address to send the returned AI generated email report to the given company's email address as a representative of Duke.ai

Note: The current version is in template format in consideration for the security of their API (I also formatted it this way since some of the assets I used to test this were tied to me personally)


About its creation:
- AI was used in the creation of this, but mostly for specifics on how to handle excel files, query ChatGPT, and use the API

- I was taught how to use the API under CEO Marcus Cooksey's instruction, he was also the one that gave me this project and internship.

- The prompt was created entirely by my own trial and error to get the emails both looking professional and using the correct subjects when addressing itself as well as the company it is talking to.

- The logic of this project wasn't too hard for my skillset, however the technical aspects, specifically API handling, is where this project was hardest since I lack substantial professional experience yet in those topics.
