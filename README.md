import random
print("Welcome to the Animal Sound Quiz!")
questions = [
 {"question": "What sound does a cat make?", "answers": ["A) Woof", "B) Meow", 
"C) Oink", "D) Moo"], "correct": "B"},
 {"question": "What sound does a dog make?", "answers": ["A) Meow", "B) Woof", 
"C) Oink", "D) Moo"], "correct": "B"},
 {"question": "What sound does a pig make?", "answers": ["A) Meow", "B) Woof", 
"C) Oink", "D) Moo"], "correct": "C"},
 {"question": "What sound does a cow make?", "answers": ["A) Meow", "B) 
Woof", "C) Oink", "D) Moo"], "correct": "D"}
]
random.shuffle(questions)
score = 0
for question in questions:
 printf("\n" + question["question"])
 for i, answer in enumerate(question["answers"]):
printf("{i+1}. {answer}")
user_answer = input("Enter your answer: ")
if user_answer.upper() == question["correct"]:
printf("Correct!")
score += 1 else:
printf("Incorrect. The correct answer is {question['correct']}.")
print(f"\nYour final score is {score} out of {len(questions)}.")



