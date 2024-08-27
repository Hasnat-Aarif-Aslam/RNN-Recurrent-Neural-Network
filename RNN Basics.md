![image](https://github.com/user-attachments/assets/9c265d8b-82f3-4e03-92e8-36c325a3b692)
![image](https://github.com/user-attachments/assets/367f66b6-3ff7-4b3a-9b86-3c72ba9befd0)


To feed our model this data, we need to vectorize it:
* OHE
  
* TF-IDF
  
* Bag of Words
  
* Word 2 Vec
![image](https://github.com/user-attachments/assets/b1994130-07ae-4dd0-9e25-46bb9299d40c)


# **`OHE`**
* The length of the one-hot encoded vector is equal to the number of unique words in the dataset because each position in the vector corresponds to one unique word. This ensures that every word has a distinct and identifiable representation in the encoded format.

![image](https://github.com/user-attachments/assets/b341768d-fa5a-44db-b7ad-5ae8d845f845)

# **`FOR ANN`**
# **`Problem with Inputs (VARYING INPUT SHAPES)`**
* when we will input the 5 unique vectors for the 1st sample to the NN, its fine, but when we want to input the 2nd sample this time the input shape will be changed, as 2nd sample has 3 unique vectors to be fed to the NN


# **`ZERO PADDING SOLUTION`**
* in this case, there are maximum number of uniques words are 5:
![image](https://github.com/user-attachments/assets/583e8a0e-acb4-4c26-8ba3-1e24c13d9e2d)

* for 2nd input there are 3 unique vectors, so 3 unique vectors will go into the NN, for the other 2 vectors we can put 0:
![image](https://github.com/user-attachments/assets/05b39ada-5bf5-4559-b006-4c81fb000336)

* for 3rd input, there are 4 unique vectors, so 4 unique vectors will go into the NN, for the other 1 vectors we can put 0:
![image](https://github.com/user-attachments/assets/3695289a-1e79-4710-9bc4-2b13f860010c)

# **`THIS IS NOT A GOOD SOLUTION, IT IS EXTREMELY EXPENSIVE:`**
* `if there are total 10000 unique words, max word vector size is 100 words, min is 5`

* `when we will input that vector size of 5, we then have to pad 95 extra vectors each of size 10000!`

* `and if we then have to predict a new sample of size lets say 200 unique words, the model will fail to do so, as it was trained on max of 100 unique vectors shape!`

# **`FURTHER PROBLEMS WITH ANN IN CASE OF SEQUENTIAL DATA`**
![image](https://github.com/user-attachments/assets/fb279706-1d38-49eb-a63d-163d6f0fc8ba)


