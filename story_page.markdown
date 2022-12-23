---
layout: page
title:  "Gender representation in the film industry"
permalink: /project/
accent_image: /assets/img/cover_pic3.png
accent_color: rgb(225, 72, 5)
---

<style>
  body {
    background-color: LemonChiffon;
  }
</style>

<style>
j { color: GoldenRod }
</style>

![image](/assets/img/movie_stereo.png)

* This will become a table of contents (this text will be scrapped).
{:toc}


## <j>Introduction</j>
Throughout the history of cinema, women and men have both often been portrayed in stereotypical ways. 

Some common women stereotypes include the mother figure, the “femme fatale” and the damsel in distress. The mother figure is a stereotype where the female character is depicted as a caring and nurturing mother, and reinforces the idea that women’s primary role is to care for the children and the home. The “femme fatale” stereotype depicts female as seductive, manipulative and dangerous. The damsel in distress is probably also one of the most represented stereotypes in cinema. Often, the female is portrayed as weak and in need of rescue by a male hero, which reinforces the idea that women are helpless and need men to protect them. 

On the other hand, male characters also have their share of clichés. Some recurrent characters include the bad boy, the bachelor and so on. Some common male character attributes include being strong and athletic, violent and aggressive, competitive, intellectually gifted.

![image](/assets/img/clichés.jpg)
*Common gender stereotypes*

The portrayal of a gender in cinema can significantly impact how women and men are perceived and treated in society and thus reinforce gender stereotypes in real life. They can even contribute to oppression of the female gender. For example, roles where women are weak and dependent on men can make it more difficult for women to be seen as strong and independent, and can limit their opportunities and choices in life.

In this little datastory, we'll study gender stereotypes in movie summaries, for different epochs and regions. 

{:.note}
While it is important to recognize and celebrate the diversity of gender identities, we will not be analyzing the representation of non-binary genders in cinema in this study because they make up a small portion of the population and lack representation in our data.

## <j>Datasets</j>

To study the representation of stereotypes in cinema, we will exploit the [CMU movies summary dataset](http://www.cs.cmu.edu/~ark/personas/), which gathers various information on the actors, characters, and the pre-processed movie summaries. From these pre-processed summaries, we can gather valuable data on the actions done by characters, and associate these actions to male and female characters.
We also enrich our data with [IMDb datasets](https://www.imdb.com/interfaces/) (Internet Movie Database) from which we can gather the cast and crew list, the main actors and actresses, and ratings of movies.

The picture below shows the dataset's movies repartition according to the countries in which they were produced, the genre to which they belong, and their release year. We observe that most of the movies are dramas, produced in USA after 1980. This will have an impact on the results we obtain, as the stereotypes depicted will mostly come from the US.

![image](/assets/img/stats_movies.png)

Women are underrepresented in cinema in many roles, including actors, directors, and writers. Despite making up roughly half of the population, women are often not given the same opportunities as men in the film industry. This lack of representation is a problem that needs to be addressed so that women can have equal access to the opportunities and benefits of working in cinema. You can check below the percentage of men and women in key cinema jobs. The high percentage of male directors and writers means that the stories and perspectives that are being told in films are largely coming from a male perspective.


<!-- ![image](/assets/img/actors_genders.png)
![image](/assets/img/dir_genders.png)
![image](/assets/img/writers_gender.png) -->

![image](/assets/img/actors_dir_gender.png)



## <j>Background stories</j>
Madison is a 15-year-old girl who lives with her parents and older brother. She attends a competitive high school and is an honors student with a passion for acting. In her free time, Madison takes acting classes and auditions for local theater productions. She has also started to build a small portfolio of professional work, including a few small commercial and film roles. Madison is a confident young woman with a dream of becoming a successful actress.

Jake is a 16-year-old boy who has always dreamed of becoming an actor. He grew up in a small town, and from a young age he was drawn to the world of acting and storytelling. Jake began acting in school plays, and as he got older he started to take acting lessons and audition for professional roles. He has already appeared in a few independent films, and he is determined to continue working hard and building his skills in order to one day play in blockbuster movies. Jake is a passionate and talented young actor with a bright future ahead of him.

Which stereotypes will affect Jake and Madison during their acting career ? How will their gender impact the roles they will get to play? 

We will explore these questions in different settings: what if Madison and Jake were born in the sixties, in the nineties ? What if they work in India, USA, West Europe ? I hope you have your popcorn ready, because it's about to get interesting ! 

![image](/assets/img/popcorn2.jpeg)

🍿The following datastory is meant to be read while eating popcorn in order to enhance the overall experience. After all, what's a good story without a tasty snack to munch on ? 
{:.note title="Warning"}

## <j>Importance of age in male and female film roles </j>


Age plays a role in the type of film an actor gets to play. Let's look at the mean actors' age in some of the main movie genres for men and women. For men, adventure, thriller and parody are the genres that have the highest mean age, and for women the genres are comedy, drama and parody. The genres that the lowest mean age are drama, romance and short films, while for women, it is romance action and musical. 

![image](/assets/img/age_genre.png)

*This plot was made by directly selecting the most frequent movie genres for men and women, that's why the list of genre is different in both plots.*
{:.note}

One other aspect that impact the choice of actor for a role is the age difference between the men and women roles in a movie. 

Historically, there has been a significant age gap between male and female characters in films, with men often being depicted as older and more established, while women are often portrayed as younger and less experienced. This is very noticeable in romance movies, especially with may-december romance movies, which are movies depicting romantic relationships where there is a drastic in age between the two characters. This means we can expect Madison to have a career in cinema earlier than Jake, and to have difficulties finding roles when she gets old.

The age gap is different depending on the movie genre. Let's have a look at some of the main genres. Action movies have the higher age difference, with a gap of about 12 years. Others genre show a difference of 6 to 8 years. Dramas present the smaller age difference, with males on average six years older than females.

<p align="center">
  <img src="/assets/img/age_diff.png" alt="image" style="width:60%">
</p>



## <j>Breaking the glass ceiling: Analysis of gender parity in leading film roles </j>

Will Madison have more chances to get less important roles than Jake during her career ? Sadly, yes. Women tend to play less important roles in general. If we consider the top-3 cast of the movies, obtained with IMDb. In the most important roles, mean first rank of womens (meaning the average position of the first woman when there is one in the movie) is significantly higher than for a man, meaning that, in general, they have a lower importance role than men. We observe that this difference was a bit smaller between 1970 and 1985, but then increased again.


![image](/assets/img/cast_importance.png)

We undersampled the men actor set to account for the data gender imbalance, so that our results are not influenced by the fact that much more men were in the data. Undersampling is a good approach when much data is available, else it would have been better to oversample women roles.
{:.note title="Method"}

Now, we look into the summaries to find the conditional probability of getting a role knowing the gender. In the summaries, the first role is defined as the characters which is the more referred to. We see that men tend to have more chance of getting the main character of the movie, while women characters 2 to 4 in decreasing importance in summary.

![image](/assets/img/role_summary.png)
 

## <j>How do actions done by men and women differ in movie summaries : overview </j>

As a first exploratory analysis, we seek the actions which have a the biggest difference in frequency of occurence between male and females. We only keep actions that appear more than a threshold frequency both for males and females so that our analysis is meaningful. Below, you can observe the top 30 actions that are much more frequent for men on the left and for women on the right. What strikes us is the number of words associated to violence for men  ("shoot", "fight", "attack", "throw", "force"...) and to love for women ("love", "marry", "seduce", "lover", "couple"). Other stereotypes are also starting to appear like the fact that women "spend" more than men, and men "order", "plan", "manage". 

![image](/assets/img/faces_stereotypes.png)

Now that we have seen that some actions are more associated to a gender, we will focus on different stereotypes via analyzing the number of occurences of actions part of specific lexical fields : [love and seduction, violence, intelligence, success](/appendix/). The more present a stereotype is in the movie summaries, the more the difference of use of the lexical field of the stereotype between male and female genders will be important. Now let's see if these stereotypes importance change in time in the summaries. 


🍿*Whoa, slow down there! I thought we were supposed to be enjoying this story together, not inhaling all the popcorn in record time...  I can't believe you polished off that whole bowl before I even made it through the firsts analyses !*
![image](/assets/img/no_popcorn.jpeg)

## <j>Differences in the stereotypes between different genres of movies.</j>

It is possible that gender stereotypes may vary between different genres of films. For example, action movies may portray men in more dominant and aggressive roles, while romantic comedies may depict women in more traditionally feminine roles. Thus, we are interested in exploring this phenomenon and understanding how gender stereotypes are represented in different genres of film. The plot below shows how the importance of our different categories of stereotypes vary accros the five most frequent genres: drama, comedy, romance, action and thriller.

Contrary to our first assumptions, the stereotypes, which we defined as the difference of action frequencies between males and females, tend to be smaller in the genre they are the most linked to. For example, the difference of frequencies of actions linked to love/seduction is smaller in the romance movie. For violence, the difference is the smallest in action movies. We think this is because in a romance movie, all main characters may potentially be described as being in love so the difference is smaller. Success difference does not vary a lot accross genres, it is always associated more to men. Men tend to be more described as intelligent than women in thriller and action movies, while in romance or comedy movies there is no difference. 

![image](/assets/img/categories_by_genre.png)



## <j>Transformations of cinema gender stereotypes through time</j>
<!-- ## <j>Let's start our journey back in time : direction the 60's !</j> -->

We now look at the evolution of our four categories of actions through times. We see that the love action frequency difference between men and women tend to become smaller between 1950 and 2010, but love actions still remain more frequent for women. The violence stereotype decreased from 1960 to 1974, then increased from 1974 to 2010. Success did not vary a lot through time, always being more associated to men. The intelligence sterotype decreased from 1950 to 1974, then increased until 2010 (+20% for men). You can observe the different trends in the plots below.


![image](/assets/img/categories_by_year.png)

Stereotypes are generally maintained through time, despite some variations. No matter the year in which our actors will play roles, we can expect them to be stereotypical.




<!-- ## <j>Now it's time to go to the 90's !</j> -->



<!-- ## <j>End of the journey : let's go to the 21st century !</j> -->

## <j>Cinema gender stereotypes: A cross-cultural analysis</j>

Gender stereotypes can vary significantly between regions of the world. These stereotypes are often shaped by cultural and social norms, as well as historical and political influences.

For example, some regions may have more traditional gender roles, with strict expectations for men and women to conform to certain behaviors and occupations. In other regions, gender roles may be more free and open to individual choice. We'll now determine if certain sterotypes are more visible in certain regions of the world.

The figure below shows the mean age of men and women in movies in USA, India and West Europe, and how it changed with time. The mean age of men and women playing in movies tends to increase since 1950 in these three region. We notice that the age gap between men and women is significantly larger in Bollywood than in Hollywood and West Europe cinema.

![image](/assets/img/age_regions_world.png)

Let's also have a look at the stereotypes in the different regions:

![image](/assets/img/categories_by_region.png)

The actions performed by men and women are generally the same in the three world regions. However, some changes can still be observed. The stereotypes in Bollywood (India) are exacerbated compared to the other regions. Women are expected to perform more actions related to love and seduction, whereas men are more violent and more subject to success. 

As a woman, Madison will be more subject to clichés in Bollywood than in other regions, even though the stereotypes are observed anyway. Same for Jake, which will maybe play more violent characters in this region of the world.




## <j>Influence of female filmmakers on gender representation in movies</j>

What happens when the director and writers of a movie include women ? Do the stereotypes still remain as important or does it change something ?

If there is one woman in the writers, we see that women tend to be significantly more successful compared to men, while if there are no women in the writers, men are depicted as being more successful. Intelligence also is more associated to women. Violence stereotype for men is reinforced and love stereotype becomes less important.


![image](/assets/img/woman_writer.png)

The same phenomenon is observable when we do the same analysis on the directors of the movies.


![image](/assets/img/woman_directing.png)

We observe that having women in important roles appears to have an impact on the portrayal of gender stereotypes. A woman writer can bring a different perspective and create more opportunities for other women. However, this does not necessarily eliminate stereotypes in the movie. In fact, men tend to be depicted as more violent in movies written or directed by a woman.

If Madi wants to act in movies in which women are depicted as successful and intelligent figures, she may want to consider appearing in more films directed by women.


## <j>What have we learned ?</j>

By checking which actions are more associated to a gender in movie summaries, we have seen that in many films, men and women are often shown playing stereotypical roles. Our analysis on movie summaries shows that men are often portrayed as being more violent and aggressive, while women are often shown as being more loving. These two stereotypes are really important but we can also find others. For example, actions linked to intelligence or success are more associated to men. These gender stereotypes are harmful because they reinforce harmful gender norms and can limit the way that men and women are perceived in society. It is important for filmmakers to strive for greater representation and diversity in their casting and storytelling in order to break down these stereotypes and create more nuanced and realistic characters. One possible solution to attenuate some of these stereotypes is to balance genders in the industry. Indeed, we saw that having women in the writers and directors of a movie could impact actions distribution within a gender.

Madi and Jake will probably experience these stereotypes. For example, Madi as a woman may find that she is more likely to be offered roles that are traditionally seen as being more suitable for women, such as romantic leads or maternal figures. On the other hand, Jake as a man may find that he is more likely to be offered roles that are traditionally seen as being more suitable for men, such as action heroes or authority figures. Anyway, we wish both of them luck !

<!-- ![image](/assets/img/The_end.jpeg) -->

![image](/assets/img/directed_by3.jpg)


Thank you for reading our datastory ! 

Big thanks to Pr. Bob West and all the TA team for their advices along the semester and especially Martin for his inputs on our project!

If you're interested in the subject your can continue by reading:

-[Using Data Science to Understand the Film
Industry’s Gender Gap](https://arxiv.org/pdf/1903.06469.pdf)

