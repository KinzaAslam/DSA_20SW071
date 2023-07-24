# KinzaAslam-Data_Science_&_Analytics_20SW071

#########################Task 1
points=int(input("Enter Your Points:"));


if  points>=1 and points<=50:
  print("Prize:Wooden Rabbit");


elif points >=51 and points<=150:
  print("Prize:No Prize");
elif points >=151 and points<=180:
  print("Prize:Water Thin Mint");
elif points >=181 and points<=200:
  print("Prize:Penguin");


  ##############################Task 2
  answer=5;


guess=int(input("Enter You guess"));


if guess < answer:
    print("Your guess is too low.")
elif guess > answer:
    print("Your guess is too high.")
else:
    print("Congratulations! Your guess is correct.")




#####################################Task 3
def calculate_tax(amount, state):
    # Define the tax rates for each state
    tax_rates = {
        'CA': 0.075,
        'MN': 0.095,
        'NY': 0.089
    }


    # Check if the state is in the tax_rates dictionary
    if state in tax_rates:
        tax_rate = tax_rates[state]
        tax_amount = amount * tax_rate
        total_amount = amount + tax_amount
        return total_amount
    else:
        print("Invalid state code. Cannot calculate tax.")
        return None


# Test the function
purchase_amount = float(input("Enter the purchase amount: "))
state_code = input("Enter the state code (CA, MN, or NY): ")


total_amount_with_tax = calculate_tax(purchase_amount, state_code)
if total_amount_with_tax is not None:
    print(f"Total amount with tax: ${total_amount_with_tax:.2f}")


    ##################################Task 4
    sentence = ["the", "quick", "brown", "fox", "jumped", "over", "the",
"lazy", "dog"]


for element in sentence:
    print(element);




    ##############################Task 5
    number_list = list(range(1, 31))




multiples_of_5 = [num for num in number_list if num % 5 == 0 ]


# Display the multiples of 5


print(multiples_of_5);






#########################Task 6 (Extracting Names)


names = ["Kinza", "Shifa", "Faiz", "Tom and Jerry", "Kashif"]
first_names = [name.split()[0].lower() for name in names]
print(first_names)






############################Task 7(Multiples of 3)
multiples_3 = [num * 3 for num in range(1, 21)]
print(multiples_3)




#############################Task 8 (PAssed or Fail)
scores = {
    "Kinza": 70,
    "Shifa": 35,
    "Faiz": 82,
    "Tom & Jerry": 23,
    "Kashif": 98
}


passed = [name if score >= 65 else name + " (Failed)" for name, score in scores.items()]
print(passed);


##############################Task 9
cast_names = ["KAmboh", "Sheikh", "Rajput", "Memon", "Arain"]
cast_heights = [72, 68, 72, 66, 76]


cast = dict(zip(cast_names, cast_heights))
print(cast)




#############################task 10
cast = ["KAmboh", "Sheikh", "Rajput", "Memon", "Arain"]
heights = [72, 68, 72, 66, 76]


for index, name in enumerate(cast):
    cast[index] = name + str(heights[index])


print(cast)







