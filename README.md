# Lab 6: Cluster Analysis

### Directions
* *Accept the Assignment*: When you accept the assignment in GitHub Classroom, a repository named `lab-06` will be automatically generated for you under the "s486Fall2023" organization.
* *Locate Your Repository*: Your personal repository for this homework can be found at `https://github.com/s486Fall2023/lab-06-your_user_name`.
* *Clone the Repository*: 
    - Open your terminal and navigate to the directory where you want to download the repository.
    - Run `git clone [your repository URL]` to clone the repository onto your local machine.
* *Working Directory*: The cloning process will create a new directory named `lab-06-your_user_name`. Ensure that you perform all your work inside this directory.
* *Commit Your Progress*: As you work on the assignment, remember to commit your changes periodically. You can easily do this using Visual Studio Code (VS Code).
* *Remote Connection*: If you've cloned the repository correctly and are working within the created directory, the remote link to your GitHub repository should already be configured.
* *Assignment*:  **The lab questions are below these directions.**  
* *File and Function Names*:
    - Please complete create a notebook file to do you work.  Answer the questions in markdown cells and keep your code neat and well documented. 
    
* You do not need to submit on Gradescope.  Just submit all your work to the GitHub repo.
  

---
## Question 1: Clustering numerical data

The "`baseball.csv`" dataset from [this GitHub repo](https://github.com/esnt/Data/tree/main/CleanData) is a subset of Lahman's Baseball Database with total hits, 
home runs, runs batted in, and stolen bases for many MLB players (`playerID`, `firstName` and `lastName` should not be used in the clustering, but they could be helpful when trying to interpret clusters.)  

1. Begin by exploring the dataset.  Create pairwise scatter plots and summary statistics.  
2. Use K-means the players into clusters based on the features.  
3. Use WCSS, silhouette scores and plots, and at least one other clustering metric to determine the how many clusters seems appropriate (consider values of $K$ from 2-6).  Justify your final choice for the value of $K$. 
4. Perform clustering using hierarchical agglomerative clustering.  Compare the dendrograms using single, complete, average and ward's linkage methods. 
5. How many clusters seem to be in the data given your analysis in part (4)?  
6. Perform clustering using Gaussian Mixture Models using the number of clusters that you found in part (3 or 5).  What are the parameter estimates determined by the model (mean and covariances of each cluster and the mixing percentages).
7. Use the results of GMM from part (6) to identify anomalies in the data. Reflect on any external factors that might explain these anomalies. 
8. Compare the results obtained from the K-means, HC, and GMM methods.  Which methods seems most appropriate for this dataset and why?
9. Select a cluster grouping from one of your clustering methods and compute summary statistics for each cluster.  Re-create the pairwise scatter plots colored by group membership. 
10. What do these statistics and plots suggest about player performance?  Give each cluster a name based on the plots and summary statistics. 
---

## Question 2: Clustering text data

The "`heath_tweets.txt`" dataset from [this GitHub repo](https://github.com/esnt/Data/tree/main/Text)
comes from the UCI Machine Learning Repository and it contains health related tweets from 16 news agencies. 

1. **Data Cleaning and Preprocessing:**  
    * Clean and preprocess the data for topic modeling. This could include removing irrelevant information (such as URLs and user handles), tokenizing the text, removing stop words, and applying stemming or lemmatization. Encode the tweets using TF-IDF or word embeddings
    * Justify your preprocessing steps. Explain how your choices might affect the outcome of the topic modeling.

2. **Topic Modeling with KMeans:**
    * Perform topic modeling using KMeans. Describe the process you used to determine the number of topics and justify your choice.
    * Identify and describe the topics you discovered. Provide representative tweets for each topic.

3. **Topic Modeling with LDA** (Latent Dirichlet Allocation):
    * Apply LDA to the dataset. Experiment with different numbers of topics and values for alpha and beta parameters. Explain how your choices impacted the results.
    * Identify and describe the topics found by LDA. Provide representative tweets for each topic.

4. **Comparative Analysis:**
    * Compare and contrast the topics identified by KMeans and LDA. Discuss the strengths and limitations of each method in the context of this dataset.
    * Based on your analysis, which method do you think is most effective for topic modeling in this context? Provide reasons for your choice.

5. **Reflection on Real-world Application:**
    * Reflect on how these topics might be useful for understanding public health trends or concerns as expressed on social media. Discuss potential real-world applications of your analysis.




 
