![image](https://github.com/ob3dd/IMDB-Movie-Predictions/assets/133266342/91616482-2377-4d0f-bbc9-e3dc836b8c40)
# IMDB Movie Predictions
## Using a MySQL database from a subset of IMDB dataset to analyze what makes a movie successful
**Obed Okoro**
# Buisness Description
Will be analyzing what makes a movie successful and will provide recommendations to the stakeholder on how to make a successful movie.
# Source of Data:
https://developer.imdb.com/non-commercial-datasets/. There were three datasets to work on, Basics with 1376640 rows and 9 columns, Ratings with 68210 rows and 3 columns and AKAS with 41+ row and 8 columns.
# Analytical Insights
During the exploratory data analysis, a barplot and countplot were visualized for each categorical column. 
- This gave a good baseline for all of the numeric and categorical columns for univariate EDA.
- A barplot was used to calculate our average revenue for each movie category
- And a heatmap was used to address our multicollinearity for a model.
![image](https://github.com/ob3dd/IMDB-Movie-Predictions/assets/133266342/4df0b850-4d04-4255-a504-8eacdba486eb)

 - From the above plot, we can deduce that;
      
        - Movies with the general audiences(G) had the modt revenue (was the highest with $133.22million average revenue)
          
        - The least was the 'restricted'(R) movie rating with $47.88million. This was probably because it wasn't suitable for kids, considering it contained some adult content/material. Usually, paeretns are urged to learn more about the adult film beiong produced under this movie rating before allowing their childrem to watch it. 
   
   ### List of movie rating systems

  - G: $133,216,900 (133.22 million)

  - NR: $43,133,930 (43.13 million)

  - PG: $129,125,600 (129.13 million)

  - PG-13: $111,101,800 (111.10 million)

  - R: $47,884,240 (47.88 million)

![image](https://github.com/ob3dd/IMDB-Movie-Predictions/assets/133266342/fd4cdf58-e136-460d-aaf6-22a84b3e3caa)

    - The movies wuth the most budget was the PG (Parental Guidance) movies. They had a budget of $51.97million
 
    - The 'Not Rated' (NR) movies were the movie with the least budget. They had a budget of $23.71million.
    (NB:- NR movies are mostly movies that weren't submitted for rating or is an uncut version of film/movie that wasn't submitted. It could also mean these movies or films that their content are not suitable for traditional ratings: In some cases, a film might contain content that is challenging to classify using traditional rating categories. As a result, it may be labeled as "NR" to indicate that it does not fit neatly into standard rating classifications.

    
   ### List of movie rating systems
   
  - G: $44,000,000 (44 million)

  - NR: $23,712,500 (23.71 million)

  - PG: $51,974,910 (51.97 million)

  - PG-13: $46,627,330 (46.63 million)

  - R: $25,477,720 (25.48 million)


# Hypothesis Test:

- Three hypothesis test were ran for our dataset and all rejected our null hypothesis (will be showing just one of them).
- Our first hypothesis test was; "Does the MPAA rating of a movie (G/PG/PG-13/R) affect how much revenue the movie generates?"
  
   ![image](https://github.com/ob3dd/IMDB-Movie-Predictions/assets/133266342/a1d5178a-1dd7-41f8-be90-20a2edddefef)
  
   - Seeing from the graph above, our G was the highest rating which affected it positively to generate $133.22million in average revenue
   - NR was the least which affected it negatively and it generated the least revenue of $43.13million

# Best Model Metrics:

 - 7 models were ran and it could be concluded that the 2nd Model was the best with a 73.4% testing score, because it met the assumptions of our Linear Regression.

 - This was the testing and training score for our model:
     - Training R^2: 0.830
     - Testing R^2: 0.734
  
# Model's Effectiveness:
Our model 2 had an R2 of 73.4%, this will allow us to trust our model more in making predictions on movie revenues.

# Summary:
Our dataset gave us an insight on how movies generated their revenues and how the ratings unpacted the average revenue a movie/film made. Our adult movies, the R and NR rated movies had lower profits due the content of the movies made. The budget set aside for these movies and the profit made weren't that much compared to the other ratings listed above.

# Recommendation
I would recommend making more movies with the G rating and PG, PG-13 movies. There more revenues would be made because of the kids and teenagers who love to watch movies, especially eye catching movies. Those adult movies may be made once in a while based on the discretion of the movie crew. Although, their maoin focis should be directed at the other ratings if they want more revenues from their movies. 

 
