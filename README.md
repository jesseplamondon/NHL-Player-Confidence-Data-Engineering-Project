# NHL-Player-Confidence-Data-Engineering-Project

## Project Overview
This project aims to introduce personality analysis into NHL scouting and drafting by evaluating prospects' confidence and psychological attributes through their interviews. The goal is to explore why certain players, like Joe Pavelski, drastically outperform their draft position and whether key personality traits—such as confidence, discipline, leadership, and resilience—play a role in long-term success.

By analyzing draft prospect interviews, we extract and assess spoken responses to measure confidence levels and correlate them with NHL performance metrics like games played (GP), goals (G), assists (A), and points (Pts).

## Hypothesis
Traditional scouting heavily relies on physical and technical abilities, but personality traits like confidence, discipline, and mental resilience may be just as important in determining NHL success. Players who exceed expectations may share common personality characteristics that were overlooked or not fully analyzed at the time of their draft.

## Methodology
### Data Collection

NHL draft prospect interviews are compiled into a dataset (player_transcripts.csv).
Each transcript contains raw responses from prospects during pre-draft media availability.
Answer Extraction & Preprocessing

Questions are removed, leaving only player responses (playerResponses.csv).
Answers are cleaned and separated to improve accuracy in sentiment analysis.
### Confidence Analysis

Each individual answer is analyzed using VADER Sentiment Analysis, producing a confidence score (compound sentiment score).
Median confidence scores are calculated for each player to reduce bias from single responses.
### Statistical Correlation with NHL Performance

Players' confidence scores are merged with their NHL statistics from drafted_players.csv.
Correlation analysis determines how confidence relates to NHL success (GP, G, A, Pts).
Additional filtering (e.g., late-round picks) can be applied to find hidden gems.
## Key Questions
Do confidence levels in prospect interviews correlate with future NHL success?
Can we identify traits that separate long-term NHL players from busts?
Are there overlooked personality-driven predictors of draft steals?
## Future Work
Expand analysis to include discipline, work ethic, and leadership using NLP.
Develop an AI-based personality profiling model to assist scouting.
Compare confidence metrics with player development paths.
## Usage
Run Confidence Model.ipynb to generate confidence scores.
There are tools in the other scripts that were used in gathering the transcript and stats data, as well as testing examples such as refined transcripts refined using ChatGPT for 2016 1st round drafted players.
## Conclusion
By incorporating personality assessment into prospect scouting, this project seeks to uncover hidden psychological traits that contribute to NHL success and help teams make more informed drafting decisions.
