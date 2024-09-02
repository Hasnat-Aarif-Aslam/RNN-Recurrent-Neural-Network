**`The "long-term dependency problem" in RNNs refers to the difficulty they have in learning and remembering information over long sequences.`**

`in the first exmple, Marathi is spoken in india (is an example of SHORT TERM DEPENDENCY)`

`RNN, CAN PERFORM WELL IN THIS CASE`
![image](https://github.com/user-attachments/assets/0621328a-5f05-4975-aa12-67564daa35cd)

**`but as the sequence becomes big, RNN's starts to suffer from LONG TERM DEPENDENCY PROBLEM WHICH IS DUE TO VANISHING GRADIENT PROBLEM & EXPLODING GRADIENT PROBLEM`**

![image](https://github.com/user-attachments/assets/9a89a0e6-7658-4a45-9b3f-41f60b831388)


 
WE HAVE AGAIN APPLIED CHAIN RULE:
![image](https://github.com/user-attachments/assets/6cf9c52d-640b-4b7d-bee3-e1b8390d6ac0)

**`DURING BACKPROPAGATION, WE CAN CONSIDER 1ST TERM (MARKED AS 1) AS SHORT TERM DEPENDENCY, WHILE THE LAST TERM (MARKED AS 3) AS LONG TERM DEPENDENCY`**

**`so when we calculate gradient, this last term (3) has less contribution (DUE TO BECOMING ZERO OR CLOSE TO 0 causing vanishing gradient) while the 1st term has the most contribution`**
![image](https://github.com/user-attachments/assets/bfab4be8-090c-452d-8fd1-da2934f159cd)


# **`SOLUTION TO LARGE DEPENDENCY PROBLEM`**
![image](https://github.com/user-attachments/assets/e6538e46-3772-4b65-be91-5199f5187ea4)


# **`PROBLEM 2: UNSTABLE TRAINING (EXPLODING GRADIENTS)`**
ususally caused due to Unstable Weight Initialization

![image](https://github.com/user-attachments/assets/75c35243-7b86-4f02-af66-1f1dfe6ba73c)

