# ZileanLeague

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6636849.svg)](https://doi.org/10.5281/zenodo.6636849)

This projects aims to predict [League of Legends](https://www.leagueoflegends.com) 5v5 Ranked Solo match results using snapshots of game stats before the 16 minute mark

> _Zilean is a League of Legends character that can drift through past, present and future. The project is borrowing Zilean's temporal magic to foresee the result of a match._

## Introduction

Zilean is a data analysis project with an accompanying python package. **The project aims to reach high accuracy predicting the outcome of a League of Legends _5v5 Ranked Solo high elo match in KR server_**. From the prediciton, draw insights on the factors that have significant impacts on the result of a match.

Different from traditional sports, esports such as League of Legends has an innate advantage of collecting data from matches. Since every play was conducted digitally, it opened up a huge potential to explore and perform all kinds of data analysis. In this project, not only is it aimed at reaching high accuracy and drawing insights to the factors impacting the result of a match. **`zilean` wishes to create a tool that can ficilitate the process of communicating with the Riot API and perform data analytical techniques** on League of Legends matches related data. 

## Data

The data is collected using the official [Riot API](https://developer.riotgames.com/apis) with the help from the python package [Riot-Watcher](https://github.com/pseudonym117/Riot-Watcher). To view the data, please visit [Zenodo](https://doi.org/10.5281/zenodo.6596322). 

The dataset contains information about all League of Legends KR server challengers (n=300) as of 2022-05-23. The account information is stored in `accounts.json`, whereas the information about the challenger league is in `kr_challenger_league.json`. 

Match data was retrieved from the 5 most recent 5v5 ranked solo matches for each challenger account. There are in total 2166 unique matches. The matches are further cleaned only to include games that last more than 16 minutes (n=2078), which are stored in `matches.json`.
