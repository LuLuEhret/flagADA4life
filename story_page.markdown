---
layout: page
title:  "Gender representation in the film industry"
permalink: /project/
accent_image: /assets/img/cover_pic3.png
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

{:.note}
While it is important to recognize and celebrate the diversity of gender identities, we will not be analyzing the representation of non-binary genders in cinema in this study because they make up a small portion of the population and lack representation in our data.

## <j>Datasets</j>

To study the representations of stereotypes in cinema, we will exploit the [CMU movies summary dataset](http://www.cs.cmu.edu/~ark/personas/), which gathers various information on the actors, characters, and the pre-processed movie summaries. From these pre-processed summaries, we can gather valuable data on the actions done by characters, and associate these actions to male and female characters.
We also enrich our data with IMDb (Internet Movie Database) [datasets](https://www.imdb.com/interfaces/) from which we can gather the cast and crew list, the main actors and actresses, and ratings of movies.

The picture below shows the dataset's movies repartition according to the countries in which they were produced, the genre to which they belong, and their release year. We observe that most of the movies are dramas, produced in USA after 1980. This will have an impact on the results we obtain, as the stereotypes depicted will mostly come from the US. 

![image](/assets/img/stats_movies.png)

Women are underrepresented in cinema in many roles, including actors, directors, and writers. Despite making up roughly half of the population, women are often not given the same opportunities as men in the film industry. This lack of representation is a problem that needs to be addressed so that women can have equal access to the opportunities and benefits of working in cinema. You can check below the percentage of men and women in key cinema jobs. The high percentage of male directors and writers means that the stories and perspectives that are being told in films are largely coming from a male perspective.


<!-- ![image](/assets/img/actors_genders.png)
![image](/assets/img/dir_genders.png)
![image](/assets/img/writers_gender.png) -->

![image](/assets/img/actors_dir_gender.png)



## <j>Background stories</j>
Madison is a 15-year-old girl who lives with her parents and older brother. She attends a competitive high school and is an honors student with a passion for acting. In her free time, Madison takes acting classes and auditions for local theater productions. She has also started to build a small portfolio of professional work, including a few small commercial and film roles. Madison is a confident young woman with a dream of becoming a successful actress.

Jack is a 16-year-old boy who has always dreamed of becoming an actor. He grew up in a small town, and from a young age he was drawn to the world of acting and storytelling. Jack began acting in school plays, and as he got older he started to take acting lessons and audition for professional roles. He has already appeared in a few independent films, and he is determined to continue working hard and building his skills in order to one day play in blockbuster movies. Jack is a passionate and talented young actor with a bright future ahead of him.

Which stereotypes will affect Jack and Madison during their acting career ? How will their gender impact the roles they will get to play? 

We will explore these questions in different settings: what if Madison and Jack were born in the sixties, in the nineties ? What if they work in India, USA, West Europe ? I hope you have your popcorn ready, because it's about to get interesting ! 

![image](/assets/img/popcorn2.jpeg)

🍿The following datastory is meant to be read while eating popcorn in order to enhance the overall experience. After all, what's a good story without a tasty snack to munch on ? 
{:.note title="Warning"}

## <j>Age gap in male and female film roles </j>


Age plays a major role in the type of film an actor plays in. As a aspiring actors, Madisons and Jake's career path will be influenced by the age trends in the different movie genre and localisation in the world. Let's look at the mean actor age in some of the main movie genres for men and women. Jake is more likely to act in romance movies, whereas Madison will probably play in musical or romance movies. As they get older, the first one will have an increasing chance to play in adventure or parody movies, and the second one romantic drama or LGBT movies.

![image](/assets/img/age_genre.png)

One other aspect that impact the choice of actor for a role is the age difference between the men and women roles in a movie. 

Historically, there has been a significant age gap between male and female characters in films, with men often being depicted as older and more established, while women are often portrayed as younger and less experienced. This is very noticeable in romance movies, especially with may-december romance movies, which are movies depicting romantic relationships where there is a drastic in age between the two characters. This means we can expect Madison to have a career in cinema earlier than Jack, and to have difficulties finding roles when she gets old.

How do the age gap changed with the movie genres ? We see that the age difference is not varying a lot accross genres, staying between 7 and 8.5 years (already a lot!), except for action movies which present a 12 years difference between men and women actors !

![image](/assets/img/polar.png){:width="70%"}



## <j>Breaking the glass ceiling: Analysis of gender parity in leading film roles </j>

...IMDb...

## <j>How do actions done by men and women differ in movie summaries : overview </j>

...fig more popular actions...

Now that we have seen that some actions are more associated to a gender, we will focus on the two most stereotyped lexical fields : love for women and violence for men. The more present a stereotype is in the movie summaries, the more the difference of use of the lexical field of the stereotype between male and female genders will be important. Now let's see how these stereotypes changed in time in the summaries.






## <j>Transformations of cinema gender stereotypes through time</j>
<!-- ## <j>Let's start our journey back in time : direction the 60's !</j> -->

What if Madison and Jack were starting off their careers in the 60's ? Well, here is a list of actions that Madison and Jack have way more chance to do compare to the others.

...add figure with strerotyped words...

We observe that ... (text with Madison and Jack)

...add violence and love logistic regression...


Now in the 90's, ...

...add figure with strerotyped words...

...add violence and love logistic regression...

And finally, in the 21st century...

...add figure with strerotyped words...

...add violence and love logistic regression...



<!-- ## <j>Now it's time to go to the 90's !</j> -->

***

🍿Whoa, slow down there! I thought we were supposed to be enjoying this story together, not inhaling all the popcorn in record time.  I can't believe you polished off that whole bowl before I even made it through the firsts analyses !
![image](/assets/img/no_popcorn.jpeg)

<!-- ## <j>End of the journey : let's go to the 21st century !</j> -->

## <j>Cinema gender stereotypes: A cross-cultural analysis</j>

Gender stereotypes can vary significantly between regions of the world. These stereotypes are often shaped by cultural and social norms, as well as historical and political influences.

For example, some regions may have more traditional gender roles, with strict expectations for men and women to conform to certain behaviors and occupations. In other regions, gender roles may be more free and open to individual choice. We'll now determine if certain sterotypes are more visible in certain regions of the world.

The figure below shows the mean age of men and women in movies in USA, India and West Europe, and how it changed with time. The mean age of men and women playing in movies tends to increase since 1950 in these three region. We notice that the age gap between men and women is significantly larger in Bollywood than in Hollywood and West Europe cinema.

![image](/assets/img/age_regions_world.png)

If Jack and Madi worked in Hollywood...

...Bollywood...

...West Europe...


## <j>Influence of female filmmakers on gender representation in movies</j>

....Separate movies written/produced by male and females and check : importance of roles of women in these movies. Most frequent actions, violence and love.....

## <j>What have we learned ?</j>

In many films, men and women are often shown playing stereotypical roles. Our analysis on movie summaries shows that men are often portrayed as being more violent and aggressive, while women are often shown as being more loving and nurturing. These gender stereotypes are harmful because they reinforce harmful gender norms and can limit the way that men and women are perceived in society. It is important for filmmakers to strive for greater representation and diversity in their casting and storytelling in order to break down these harmful stereotypes and create more nuanced and realistic characters.


![image](/assets/img/The_end.jpeg)

![image](/assets/img/directed_by.jpg)


Thank you for reading our datastory ! 

Big thanks to Pr. Bob West and all the TA team for their advices along the semester and especially Martin for his inputs on our project!

If you're interested in the subject your can continue by reading:

-[Using Data Science to Understand the Film
Industry’s Gender Gap](https://arxiv.org/pdf/1903.06469.pdf)

