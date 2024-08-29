**`A SIMPLE RNN, CAN STORE THE MEMORY OF LAST 1O TIME STEPSS`**

![image](https://github.com/user-attachments/assets/09675815-b701-4f2f-b7f8-8d713771f1c9)

**`In keras we use this format to input data in RNN:`**
* 3 represents, we want to input 3 samples from our dataset
![image](https://github.com/user-attachments/assets/363f6ab5-cb0b-4c69-b646-02603365fff5)


**`WORKING`**
![image](https://github.com/user-attachments/assets/c8403a81-a472-42b2-a8b6-20f1c0f1d235)
* in ANN, the data only flows forward during input

* in RNN, we will input the 1st sample as X11 at time_step = 1 or 0

* then we will input X12 of 1st sample at time_step = 2 and so on

* there is a concept of `STATE` in RNN


**`ARCHITECTURE`**
![image](https://github.com/user-attachments/assets/99a24951-fe15-4e90-a6ea-128254f5d56d)
![image](https://github.com/user-attachments/assets/eb856f08-7b57-4838-9d13-0c31ecc126d8)


**`Code`**
![image](https://github.com/user-attachments/assets/16b0061d-f67a-445e-a084-e9d5b8dbb13f)
![image](https://github.com/user-attachments/assets/edc04854-ae44-491e-99e8-d4459ac86f47)
![image](https://github.com/user-attachments/assets/23dc5484-283c-44da-a967-fda5149567b9)
![image](https://github.com/user-attachments/assets/621c708e-ae0e-41f1-b17e-4cd2971cf796)
![image](https://github.com/user-attachments/assets/30198615-93bd-4ed7-9820-aa79e77779a3)



**`FORWARD PROP.`**
![image](https://github.com/user-attachments/assets/0e0719bc-f6cf-4af6-8a5f-5e8b6b5654d9)
![image](https://github.com/user-attachments/assets/7de41763-b478-4e35-bf22-a0ca63ee8cc6)

![image](https://github.com/user-attachments/assets/bbb2e9d5-e9ec-45d8-ba97-6cd06747a4e2)



