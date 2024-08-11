# SQL-query-Statements-1

### Project Overview 
To showcase different sql functions and their various meanings

### Data Source
The data "dbo.players" was gotten from POSHEM TECHNOLOGIES 

### Tool
The tool used for this project is Microsoft Server Query Language (MSSQL)

### Exploratory Data Analysis

The EDA involved exploring the dbo.players data to answer different questions
 ##### Question 1. 
 -  Write a query to display all the information inside players.
 -  Write a query to retrieve the last_name, first_name and city for each player.
 -  Write a query to retrieve the email_address, country, and street_address for each player. 
 -  Write a query to display the player_id, total_playing_minutes, and installed_games for each player.
 -  Write a query to display the player_id, age_group, and total_playing_minutes for each player.

##### Question 2.
- Write a query to display for each player - the player_id, amount_spent_usd, and a new calculation representing the amount spent in euros, with exchange rate of 0.8.
- Write a query to display the player_id, last_name, first_name, amount_spent_usd, installed_games, and a new calculation representing the average amount spent on each game (amount_spent_usd / installed_games)
- Write a query to display for each player - the player_id, email_address, installed_games, uninstalled_games, and a new calculation representing the ratio between installed and uninstalled games (uninstalled_games / installed_games)

##### Question 3. 
- Write a query to display the:
1.  player_id
2.  player's first_name concatenated with his/hers last_name

- Write a query to display the:
1. player_id
2.  email_address
3.  country concatenated with city and street_address
4.  total playing time in hours (total_playing_minutes / 60)

##### Question 4. 
- Write a query to display the following string for each player:
(Full name preferred language is preferred_language)

##### Question 5.
- Write a query to display the distinct values inside the preferred_language column
- Write a query to display the distinct list of values inside the gender column
- Write a query to display the distinct list of values inside the age_group column
- Write a query to display the distinct combination of gender and age_group columns

  ### Data Analysis
Some of the queries written to answer these questions are;

  ```MSSQL
  select * from dbo.players;
  ```

  ```MSSQL
  select last_name, first_name, city from dbo.players;
```

```MSSQL
select player_id, age_group, total_playing_minutes from dbo.players;
```

```MSSQL
select player_id, last_name, first_name, amount_spent_usd, installed_games, (amount_spent_usd / installed_games) as average_amount_spent from dbo.players;
```

```MSSQL
select player_id, concat(first_name,'  ',last_name) as full_name from dbo.players;
```

```MSSQL
select distinct gender from dbo.players;
```

