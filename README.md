# NFL-Contract-Draft-Data-2000-2022
NFL Contract &amp; Draft Data 2000-2022

Every contract a player has signed appears as it's own row in this dataset along with information about when and who they were signed to. Joining of the contract and draft data was done via fuzzywuzzy off of the player name and position. Players with common/duplicate names should be scrutinized or excluded and their contract and draft data may have misjoined.

This streamlit app allows for some exploration of the data: https://nfl-contracts.streamlit.app/

Dictionary:

draft_year: the year they were drafted

rnd: the round they were drafted in

pick: the pick # they were selected at

tm: the team that drafted them

player: the name of the player

g: the number of games the player played in their career

search_key: the key that was used for joining, retained as it could be valuable for displaying

year_signed: the year the contract was signed

signing_tm: the team that signed them (this needs to be cleaned to match with 'tm')

value: the total US dollar value of their contract at signing (not adjusted for inflation)

gtd: the total US dollar guaranteed value of their contract at signing (not adjusted for inflation)

value and gtd were normalized to the NFL salary cap for that year (value_norm and gtd_norm). This allows for comparison of contract values across years since the salary cap (generally) increases every year roughly aligned with inflation.
