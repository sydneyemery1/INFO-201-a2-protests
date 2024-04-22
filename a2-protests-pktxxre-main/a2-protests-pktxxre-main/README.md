# Assignment 1: Protests

During the past few years in the United States, there has been a surge of protests in support of the Black Lives Matter movement, women's rights, trans rights, immigration reform, gun control, the environment, and many other social and political issues.

In this assignment, you will work with data from [CountLove](https://countlove.org/), a group that collects data about protests from across the United States, including information about the purpose of the protests, the location of the protests, as well as how many people attended the protests. This data has often been [cited by the *New York Times*](https://www.nytimes.com/2020/08/28/us/black-lives-matter-protest.html), among other major outlets.

Through this assignment, you will be able to answer questions including:
- What were the most attended and least attended protests in the US in the last 5 years?
- How many protests occurred in Washington state?
- How did the number of protests in 2019 compare to 2020, and why?
- Why are people protesting in the US? What are the biggest motivators?


This assignment is divided into 2 parts. You will complete your coding work in the `analysis.R` file, and you will write short answer responses related to critical analysis and reflection of the data in this `README.md` file. Before getting started on your coding work, you should complete the section **"Critical Analysis & Reflection: Before You Code"** below.

When you are finished with the assignment, be sure to push all changes to your GitHub repository and then submit the link on Canvas.

## Before You Code: Critical Analysis & Reflection

Before diving into this (or any) dataset, it's important to know where the data came from, and it's important to have or to seek out _domain familiarity_ — in other words, knowledge about the subject/topic of the dataset. (We don't want to be "strangers in the dataset," as Catherine D'Ignazio and Lauren Klein describe it.)

To get more familiar, we are going to begin by doing some background reading.

- First, please read [this FAQ](https://countlove.org/faq.html) from the CountLove website and the opening of [this blog post](https://www.tommyleung.com/countLove/index.htm). Based on the information in these pieces, why did the creators start collecting the CountLove data? Please answer in 2-3 sentences (3 points)
The creators started collecting data from the CountLove data in order to better display the numbers that are applicable to protests. These numbers include that of the numbers of locations that protests take place along with the times that they take place and the number of people that are in attendance. With note made of how having factual representations of this data is incredibly valuable to citizens, politicians, and journalists, the work done by the creators seems to be done to provide cival benefit. 

- Next, we would like you to read this [*New York Times* piece, which uses CountLove data](https://www.nytimes.com/interactive/2020/06/13/us/george-floyd-protests-cities-photos.html) (here's a [Google Doc version for anyone who gets paywalled](https://docs.google.com/document/d/1sdjFsA5csYuH4plNEEk7WXT77K5h5ZuyW05CBwYdk6A/edit?usp=sharing)), and which describes the Black Lives Matter protests that occurred in the summer of 2020. Please summarize the main point or argument of this article in 2-3 sentences (3 points)
The main point that is seen is that of how communities came together to support each other and advocate for the rights of George Floyd and others that have experienced unjust situations corresponding with race. The protests that were discussed in the article denote those that took place across the United States, ranging from small towns to huge cities, and ranging from average incomes of $20,000 to $220,000, showing the range of impact that this movement has. 
  

Next, we're going to reflect about who collected this data, and what's actually inside it.

- Who collected and shared the CountLove data, and what do they do for a living? Please answer in 1-2 sentences(2 points)
Tommy Leung and Nathan Perkins, who met while pursuing their Masters in Technology and Policy at MIT, are the two people who collected and shared the CountLove data. 


- As Klein and D'Ignazio remind us, when it comes to data, "what gets counted counts." What types of demonstrations does CountLove include in their data, and what types do they exclude? (3 points)
The types of demonstrations that CountLove includes in their data are that the protests aren't part of what is deemed "regular business." For what is excluded from the protest data collected by CountLove is that of reenactments, political campaign rallies, and the likes of awareness events. 
  

- How and where does CountLove get their data about the protests? Please answer in 2-3 sentences (2 points)
The CountLove team gets their data about the protests from local newspapers and television sites. The inital data that was used for the 2017 Women's March came from the Crowd Counting Consortium. 


- How does CountLove make their estimates about the number of people who attended a protest? What potential problems might arise from this method of estimation? Please answer in 3-4 sentences (4 points)
CountLove makes their estimates about the number of people who attended a particular protest by making the most conservative attendance estimate. It is stated that the CountLove team interprets a "dozen" as being ten, "dozens" as being 20, and "hundreds" as one hundred. Should an article only mention the deonstration at a protest rather than an actual attendance number, the attendance count is left empty. 


## While You Code: Critical Analysis & Reflection

- Reflection 1: Why do you think the mean is higher than the median? Which metric would you use in a report about this data, and why? Please answer in 2-3 sentences (2 points)
I think that the mean is higher than the median because of a few high value points that are skewing the data. I would use the median because it will be a more accurate demonstration of the data as it is not impacted by outliers. 

- Reflection 2: Before actually calculating the number of protests that occurred in 2018, 2019, 2020, record your guesses for the following questions. (1 point)

  Guess: Do you think there were more protests in 2019 than in 2018? Why or why not? Please answer in 1 or 2 sentences
  I think that there were more protests in 2019 than 2018 because with every year, human rights were becoming more and more an open topic of conversation. 

  Guess: Do you think there were more protests in 2020 than in 2019? Why or why not? Please answer in 1 or 2 sentences
  I think that there were more protests in 2020 that 2019 due to the pandemic seeing that there were events occuring that amplified the conversation of human rights. 

- Reflection 3: Does the change in the number of protests from 2018 to 2019 to 2020 surprise you? Why or why not? What do you think explains the fluctuation? Please answer in 1 or 2 sentences (2 points)
The change in numbers does surpise me as I was not expecting there to be a greater number of protests in 2018 than 2019. What I think explains this fluctuation is perhaps other occurances that were taking place, like that of womens rights rather than just the number being based off of the black lives matter movement. 

- Reflection 4: What is the first and fourth most frequent category of protest? Do these frequencies align with your sense of the major protest movements in the U.S. in the last few years? Why or why not? (3 points)

The first most frequent category of protest was racial injustice and the fourth most frequent protest was civil rights. I think that this aligns with my sense of major protest movements that occured in the U.S. in the last few years. I believe that this is because of the movements surrounding individuals like George Floyd, which allowed for light to be shed on the injustice that many people face in their daily lives. 

## After You Code: Critical Analysis & Reflection

In the second chapter of *Data Feminism*, Klein and D'Ignazio describe 4 ways that data scientists can challenge power and take action:
> Taking action can itself take many forms, and in this chapter we offer four starting points:  
> (1) Collect: Compiling counterdata—in the face of missing data or institutional neglect—offers a powerful starting point as we see in the example of the DGEI, or in María Salguero’s femicide maps discussed in chapter 1.  
> (2) Analyze: Challenging power often requires demonstrating inequitable outcomes across groups, and new computational methods are being developed to audit opaque algorithms and hold institutions accountable.  
> (3) Imagine: We cannot only focus on inequitable outcomes, because then we will never get to the root cause of injustice. In order to truly dismantle power, we have to imagine our end point not as “fairness,” but as co-liberation.  
> (4) Teach: The identities of data scientists matter, so how might we engage and empower newcomers to the field in order to shift the demographics and cultivate the next generation of data feminists?  

- How does the CountLove project embody one or more of these 4 forms of challenging power? Please answer in at least 3-4 sentences (3 points)
One way that COuntLove embodies one or more of the four forms of challenging power is in how teaching is used to visually demonstrate to an audience the power that comes with the data at hand. Given how CountLove discusses one of their points of focus was creating their data for politicians and the public. With these groups having the ability to see the ways in which communities are being impacted through the cause that they actively support, this allows for politicians to better advocate for the communities they represent and for people to come together to support causes they feel passionately about. 

- What is the most interesting or surprising thing you learned from this analysis? Please answer in at least 2-3 sentences (2 points)
The most interesting thing that I learned about this analysis was how even in areas that are deemed more rural, people still came together to advocate for causes. Though these groups were seen to be smaller than in larger cities, the analysis shows that overall, there was still impact that these people brought about by their ultimate contribution. 

- What is a kind of analysis that you would like to do or that would be interesting to do with the CountLove data that you don't have the time or skills to accomplish at this moment? Please answer in at least 2-3 sentences (2 points)
Something that I would be interested to do with the CountLove data would be to see what protests have the most impactful outcomes. Whether this comes in the form of impacting the thinking of one person that then came positively impact the lives of 20 others in a smaller community, or whether the motives of a large corporation were swayed, I would be curious to see the impact that was felt.