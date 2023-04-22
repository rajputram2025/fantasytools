# Fantasyer

## DESCRIPTION 

The project aims to develop a fantasy helper application – to provide stats of players and teams to help build the right team on Fantasy. Match data and ball by ball data scrapped data from cricsheet are used in calculating essential stats for batters and bowlers.The front end is built using StreamLit and deployed using Google sheets and StreamLit.

## SOFTWARES AND DEVOP TOOLS USED

- Jupyter Notebook
- Visual Studio Code

## LANGUAGE USED

- Python

## FEATURES

For selecting the right team on fantasy applications, a lot of factors need to be considered, including toss, combination of both teams, stats of players and of course a little bit of luck to go your way. The 11 members chosen must maximize your profits, minimize risks and also be a little different from every other team picked by others. In this API, we have configured a few features that would help you make an informed decision about picking the team.

#### TOSS

One of the most important factors to consider is the toss, especially in a t20 game in Asia were dew plays a massive role. We use the match data for all seasons in the IPL from 2008 to 2022 and calculate a few important stats that need to be considered to decide the balance of your side (6-5/ 7-4 skewing towrads the chasing / defending team)

###### TOSS VS VENUES
- Is the toss that important in T20 games, does chasing have a significant advantage.
- Find out toss outcomes and game outcomes in specific venues - Just click the drop down list box and choose the stadium
- You will find the what the majority of teams winning the toss here have chosen to do. 
- You will also see the percentage of matches won by the team that won the toss

###### TOSS VS SEASON
- 2021 IPL had a massive skew to chasing because of the slow surfaces used in UAE.
- Surfaces change across seasons and therefore it is important to understand the trends of the current season
- Find out the trends of the ongoing season of IPL - bat first / bowl first

###### TOSS VS YOUR TEAM
- Few captains win more tosses than the others which gives a massive advantage while playing in Asia
- For this reason, knowing the match win percentage while your teams win the toss proves to be an important factor
- Find out if your team wins if they win the toss. Also, find out how much your team wins the toss.

###### TOSS VS OPPOSITION
- SRH love defending, GT love chasing
- Knowing your opposition's strength is valuable to decide the balance of your side
- Find the strength of your opposition. Are they a SRH or a GT

#### PLAYER IN GROUND STATS
- Batters and bowlers like certain venues and dont like certain venues. 
- Rohit Sharma loves Eden Gardens, Shubman Gill hates Wankhade
- This depends on how the conditions suit their style of play
- Just give the name of the batter and the bowler with the venue, stats like average, strike rate, boundary percentage will be printed for batters and stats like average strike rate, economy will be calculated for bowlers.

#### PLAYER VS OPPOSITION STATS

- Similar to grounds, players also have favorite oppositions.
- David Warner loves KKR, Tewatia loves Punjab Kings
- Just give the name of the batter and the bowler with the opposition, stats like average, strike rate, boundary percentage will be printed for batters and stats like average strike rate, economy will be calculated for bowlers.

#### PLAYER VS TEAM STATS

- How well a player plays against an opposition also depends on how well he plays the main bowlers of the attack/ how well he bowls to the top batters of the team
- This might be similarv to player vs opposition, but due to the mega auction in 2022 and the addition of 2 new teams, bowling and batting core has changed.
- Just give the name of the batter and the bowler with the opposition, stats like average, strike rate, boundary percentage will be printed for batters vs each of their team's bowlers and stats like average strike rate, economy will be calculated for bowlers vs each of their team's batters.


## FEATURES TO BE DONE

Future enhancements
- Batter records vs bowling type(LAP/RAP/SLA etc) in different phases
- Bowler vs RHB/LHB in different phases

Addition of Fantasy articles
- Articles on batter, bowler and team form
- Other matchups that might help

## DATA

- https://cricsheet.org/ has maintained matches data and ball by ball data of all IPL matches in yml format. 
- These files have been taken and converted to CSV's. 
- The folder archive has all the data files we need - https://github.com/charanya78/fantasyer/tree/main/archive

## FRONT END DESIGN
Streamlit is used for visualizing the project and each feature is categorized under separate tabs

Example 1:

![image](https://user-images.githubusercontent.com/59957617/208448016-969292b9-9cab-424d-b199-b7b4e29d90f7.png)

Example 2:

![image](https://user-images.githubusercontent.com/59957617/208448113-452423f3-4c17-4673-8f87-ac62cefa8722.png)

The following functions from streamlit are majorly used:
- <i>selectbox</i>  : To display drop down options
![image](https://user-images.githubusercontent.com/59957617/208449293-f38108e9-e09a-4b93-af22-c643ac644710.png)

- <i>markdown</i>   : To display text with formatting
![image](https://user-images.githubusercontent.com/59957617/208449387-6447d3c5-5e0f-47df-a3a9-62df11f32c1d.png)

- <i>dataframe</i>   : To display dervied data in tabular format
![image](https://user-images.githubusercontent.com/59957617/208449504-19f85139-b00e-43a6-a450-d7c628302152.png)

## DEPLOYMENT
- For deployment purposes, StreamLit was used.
- A StreamLit account was created and the csv files used were pushed to Google sheets and their access was made public
- Requirements.txt file was added
- The app was configured in StreamLit and deployed
- Live Link : https://charanya78-fantasyer-streamlitui-streamlit-4v9psj.streamlit.app/

## EXECUTION 
- To run the app in your local system, install streamlit and the required dependencies - https://github.com/charanya78/fantasyer/blob/StreamLit/StreamLit/requirements.txt
- Navigate to StreamLit branch to the StreamLit folder
- Use the command streamlit run UI.py to run the app

