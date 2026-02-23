# DSC234 Inside the Machine: AI Literacy - Lesson Plan Weeks 6-7

**Topic:** K-Means Clustering - Unsupervised Learning From Data (Data Classification) and K-Nearest Neighbors

## Vocabulary:

**supervised learning:** In supervised learning, the computer is given both input data and correct output data. It learns to make predictions or decisions based on this labeled data.

**unsupervised learning:** Unsupervised learning is when a computer learns from data without being told what to look for. It discovers patterns and relationships all on its own.

**k-means clustering:** K-means clustering is an iterative method used to group similar things together in data. It's like sorting marbles into different boxes based on their similarities. The value of k is the number of groups or clusters.

**k-nearest neighbors:** Used in machine learning (both regression and classification) to make decisions about a test input. The value of k is the number of "nearest objects/points" that get a vote (the larger the value of k, the more members of the training data are identified as influential toward determining the outcome.

## Learning Outcomes:

The student will:
- apply essential components of a K-means algorithm to classify data.
- evaluate the process and discuss any assumptions made, human judgment versus machine processing, and effectiveness if humans are removed from the process.
- discuss how purely unsupervised learning depends on good training data.
- consider times when human intuition might be necessary and computers failed.
- describe and compare K-means with K-nearest neighbor - how they work and what they are used for in classifying and grouping data.

## Materials Needed:

- Ruler, Yarn Pieces (colors match star colors) (1 set per student), Colored Stars (3 per student)
- Sticky Notes
- Monster data handout (monster "cards", data table, graph coordinate plane, training and testing data)

## Background:

I wrote a Python script to do the "K-Means" Cluster Selection on this data, which we are calling the "training data". Without knowing what the end result should be, the algorithm had to run through the placement of each cluster center (which is called a **centroid**) 4 times before reaching the final positions. Then, I wrote the code to perform what is called a "principal component analysis" for the purposes of reducing 6 dimensions to 2 dimensions.

**The challenge:** (warmth, eyes, feet, teeth, solid, wings) <-- a vector with 6 components has 6 dimensions and if we try to plot this, it is hard to visualize.

(Last time, we tried to focus entirely on two aspects for each data point (each creature). This was a good starting point for practice. Let's take it further.)

---

## Instructions [K-Means Clustering (Part I)]:

1. Pretend you are a computer that needs to learn how to sort monsters into groups! Look at your monster bank. We need to start by identifying characteristics that we deem important, and how we will measure the importance of these features.

   The color of the monster has been converted to a number based on "warm-to-cool" scale. Look at your handout. That number is called "warmth". Then we have the number of eyes, feet, and teeth. Is the monster a solid color? 1 = yes, 0 = no. Does the monster have wings or other appendages? 1 = yes, 0 = no

   Let **X = Warmth** and **Y = 0.5 × (Eyes + Feet) - 0.7 × Teeth**

   **Q1:** What characteristics are we considering important? ______________________________

   **Q2:** What characteristics are we choosing to ignore? _______________________________

2. Calculate ( X, Y ) for all 15 monsters and plot the coordinates on the graph provided. (Did any of them end up at the same point?)

3. Select 3 "star" tokens (for sake of instruction, let's assume yellow, pink, and blue). Suggestion: place Star 1 at coordinates ( –1, –1 ), Star 2 at ( 2, 1 ) and Star 3 at ( –1.5, 2 ).

   This represents your initial (best) guess about where the 3 clusters will be located. Think of them as magnets that are attracted to data.

4. Now calculate each monster's best star. Using an actual ruler, measure the (Euclidean) distance from each monster to each star. You should have 3 distances to write down per monster.

   **This is exactly what K-means does!**

   - Make sure to measure to the center of each star token! Take 3 measurements just to be sure.
   - You will be assigning each monster to its nearest star.
   - Measuring all 3 distances will matter later, especially if there are "close" calls.
   - **This step is called the assignment step in K-means!**

   | Monster ID | Distance to Star 1 | Distance to Star 2 | Distance to Star 3 |
   |------------|-------------------|-------------------|-------------------|
   | M1         |                   |                   |                   |
   | M2         |                   |                   |                   |
   | M3         |                   |                   |                   |
   | M4         |                   |                   |                   |
   | M5         |                   |                   |                   |
   | M6         |                   |                   |                   |
   | M7         |                   |                   |                   |
   | M8         |                   |                   |                   |
   | M9         |                   |                   |                   |
   | M10        |                   |                   |                   |
   | M11        |                   |                   |                   |
   | M12        |                   |                   |                   |
   | M13        |                   |                   |                   |
   | M14        |                   |                   |                   |
   | M15        |                   |                   |                   |

5. Use your colored yarn to make a loop around all points included in a star cluster. Use the same color yarn as the color of the star. All monsters should be accounted for. Check to see that there is at least one monster in every star cluster. Stars with no monsters are called "dead clusters". We can't have that!! Since we used human intuition on the initial placement of stars, we should be ok to proceed to the next step.

   **Worth noting:** If we were using true unsupervised learning and creating clusters based only on the existing data, we would not be assigning k = 3 just yet. But, as it turns out, the choice of k = 3 is a good one.

6. Now calculate the **centroid** of each region. This is not the geographic center because we have actual (discrete) data. To use a map analogy, we are calculating the population center. Using only the ( X, Y ) values for monsters in the cluster, calculate meanX and meanY. [That is pseudocode for "mean of X" and "mean of Y"]. To calculate the mean, add up the values and divide by the number of X's. Do the same for the Y's. Write that down as coordinates: ( meanX, meanY ). You just found the **centroid** of the cluster!

   **Question 1:** Can you guess what we are going to do with the centroid?

7. This is what we call the **iteration step**. If any stars were moved to a new location, we need to remove the yarn and repeat Steps 4 - 6! Monsters that were near a boundary between clusters are vulnerable to being placed in a different cluster. We must make sure to include monsters with their nearest star!

   No stars were moved? Great! Move on to Step 8...

8. Take a photo of your cluster configuration.

### Before we move on to Part 2, we have some questions:

**Question 2:** Why was this not a true unsupervised learning approach? What assumptions did we make (say... at the beginning) that may have affected the outcome? 

_______________________________________________
____________________________________________________________________________________________________________
____________________________________________________________________________________________________________
____________________________________________________________________________________________________________

**Question 3:** Our human judgment is important. Can you think of a time in history (or two) when a human went with intuition (or common sense, or just plain daring) rather than trust a computer... and it turned out to be the right decision?

**Question 4:** Did the clusters end up the way you expected? Suppose we wanted to use this kind of algorithm to identify a child versus an adult from a photo. What are some of the concerns you have? What could go wrong? Are there any privacy or parental issues that would need to be addressed?

---

## Instructions [K-Nearest Neighbor (Part II)]:

### Introduction:
Here is where we reset the board (so to speak). Start with a coordinate plane. With the monster cards (images) of the original 15 monsters, group them according to their appropriate cluster. Think about what makes each cluster unique.

**Cluster 1** - (M7, M10) We could call this the "toothy" outlier group. Coloration is on the "cool" side, they tend to have a higher tooth count. Interestingly, they were both a turquoise color.

**Cluster 2** - (M4, M5, M6, M8, M9, M12, M14, M15) This is the largest group. Predominantly "cool to cold", non-solid, no wings or other protrusions

**Cluster 3** - (M1, M2, M3, M11, M13) This is the "warm monster" cluster and they tend to have high "eye" counts

Refer to Page 6 of the Handout for the Test Monster Data. We have the characteristics, then we "center" the values by subtracting the mean. Then we calculate the ( X, Y ) coordinates as follows:

### Step 1:
*Pick at least 6 of the monsters* and calculate by hand their projected ( X, Y ) coordinates using:

**PC1** = (−0.9293 × Warmth*) + (−0.3091 × Eyes*) + (+0.1315 × Feet*) + (−0.0930 × Teeth*) + (−0.0711 × Solid*) + (+0.0997 × Wings*)

**PC2** = (−0.0155 × Warmth*) + (+0.5213 × Eyes*) + (+0.4463 × Feet*) + (−0.0975 × Teeth*) + (−0.1745 × Solid*) + (+0.1087 × Wings*)

(= centered value)*

> Note: I used claude.ai to print out these formulas.

List the ( X, Y ) calculations and results here: ____________________________________________________________

________________________________________________________________________________________________________________

________________________________________________________________________________________________________________

### Step 2:
Refer to Page 4 of the Handout. It shows you where the *original 15 monsters* should be graphed, after conducting the K-Means Cluster algorithm. And it shows which clusters they belong in. Place them on your new graph now and label them using the M1, M2, etc names we gave them before. Also, place the stars (centroids).

### Step 3:
Start with the projected ( X, Y ) coordinates for TestM1. Place a dot (point) for it on the graph.

Now, you will use a method called "K-Nearest Neighbors" to decide what cluster the test monster belongs in. We are going to let K = 3 first, then K = 4, then K = 5. And compare the results.

- For **K = 3**, the task is to locate the 3 nearest monsters to TestM1 from the original set. The cluster belonging to the majority (2 out of 3) is the assigned cluster for K = 3.

- **K = 4**, locate the 4 nearest monsters. If there is a tie, choose the cluster of the 2 monsters with the smallest total distance to our TestM1. Assign the cluster for K = 4.

- **K = 5**, locate the 5 nearest monsters. Assign the cluster of the majority for K = 5.

**Repeat this process for all 17 monsters!**

You should have 3 things written down for each monster - the K = 3 cluster, the K = 4 cluster, and the K = 5 cluster.

### Step 4:
Decide if the model is **stable** for all test data. In other words, did the model predict the correct cluster for all values of K? Or did it change on any of the monsters?

____________________________________________________________________________

______________________________________________________________________________________________________________

### Step 5:
Consider Test monster "TestM15". What is the best approach for determining its cluster?

**For discussion:** TestM15 is warm which pulls strongly toward Cluster 2. But it has 4 teeth — the highest possible value — which is the defining trait of Cluster 0. And it has wings and 3 feet which are more Cluster 1 traits. It's genuinely a combo of all three clusters, which is why the algorithm couldn't make up its mind.

The question then becomes: does the overall "feel" of the creature — warm, winged, one-eyed — outweigh its very toothy mouth? There's no wrong answer, which makes it a rich conversation. The deeper lesson is that ambiguous cases exist in real data, and that's not necessarily a failure of the algorithm; it could absolutely be the fault of the training data — how could we determine if the algorithm failed?

---

## Comprehension and Reflection (Quiz grade)

**Question 1:** In your own words, explain the difference between the K in K-Means clustering and the K in K-Nearest Neighbor. They are both called K, but they mean very different things in each algorithm. What does each one control?

**Question 2:** Look at your final cluster assignments from Part 1 (your hand-drawn version using Warmth and the Y formula) and compare them to the algorithmic results from Part 2. Did your intuitive approach agree with the computer? Where did it agree, and where did it differ? What might explain any differences?

**Question 3:** Monster 15 was unstable — it changed cluster assignments depending on the value of K in KNN. Looking at M15's characteristics, why do you think the algorithm had trouble making up its mind? Use the actual feature values in your answer.

**Question 4:** Think about everything we have said about "machine learning" since the start of this course. Look back in your notes for assistance. After this week's two-part activity, has your concept of "machine learning" changed at all? Make a list of concepts you associate with ML.

**Question 5:** Was there a moment during this activity that something "clicked" for you, where something suddenly made sense that hadn't before? Describe that moment.

**Question 6:** What was challenging about this activity? Can you think of ways you overcame those challenges? Describe them here.

**Question 7:** Write some thoughts about human decisions that were made throughout this activity. How did that change any of the outcomes? Did you find yourself disagreeing with the algorithm? Explain any differences here.

---

## Selected Solutions (from Part I):

**( X, Y ) from Step 2:**
- M1 ( 1, 1.1 )
- M2 ( 2, –0.4 )
- M3 ( 2, 2.5 )
- M4 ( –1, 1.5 )
- M5 ( –2, 0.8 )
- M6 ( –2, 1.6 )
- M7 (–1, –0.1 )
- M8 ( –1, 2 )
- M9 ( –2, 2.3 )
- M10 ( –1, –1.6 )
- M11 ( 1, 0.4 )
- M12 ( 0, 2.5 )
- M13 ( 2, 2.1 )
- M14 ( 0, 3 )
- M15 ( –1, 2.3 )

**Step 6:** Centroid 1 (Yellow) is the average X's and Y's of M7 (–1, –0.1 ), and M10 ( –1, –1.6 )... so Centroid1 is ( –1, –0.85 ). VERY near our initial placement of the yellow star (Star1)

The five monsters in Cluster 2 were M1, M2, M3, M11 and M13. Centroid2 is ( 1.6, 1.14 )

Centroid 3 is at ( –1.125, 2 )

---

## Answers to Activity Questions:

**Question 1:** Can you guess what we are going to do with the centroid? 

**Answer:** Move the star to that location. The star needs to be located at the centroid of its cluster.

**Question 2:** Why was this (Part I) not a true unsupervised learning approach? What assumptions did we make (say... at the beginning) that may have affected the outcome? 

**Answer:**
- **We chose what X and Y are.** We decided that Warmth, Eyes, Feet, and Teeth were the relevant features, and we chose a specific formula combining them. A truly unsupervised approach like PCA lets the data tell you which features matter and how much to weight them.
- **We chose k = 3.** We assumed there were 3 clusters before looking at the data at all. True unsupervised learning would discover the number of natural groupings on its own — or at least use something like the elbow curve to inform that choice rather than declaring it upfront.
- **We chose the coefficients in Y.** The ½ and 0.7 weights were our intuition, not derived from the data. Different weights would have placed the monsters differently on the graph and potentially produced different clusters.
- **We chose which features to ignore.** Solid and Wings never appeared in our X or Y formulas at all. We made a human judgment that they weren't important.
- **We chose initial placements of the 3 stars based on intuition.** This should not have affected the outcome much, but it certainly can reduce the number of iterations required to arrive at the convergence (solution).

**Question 3:** Our human judgment is important. Can you think of a time in history (or two) when a human went with intuition (or common sense) rather than trust a computer... and it turned out to be the right decision? 

**Some possible answers:**
- Stanislav Petrov (1983)
- Lee Sedol v AlphaGo (2016) Game 4
