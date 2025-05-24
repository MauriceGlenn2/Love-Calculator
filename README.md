# 💘 Love Calculator

💪 This is a difficult challenge! 💪

You are going to write a function called `calculate_love_score()` that tests the compatibility between two names.

## 💡 Instructions

To work out the love score between two people:

1. Take both people's names and check for the number of times the letters in the word **TRUE** occur.
2. Then check for the number of times the letters in the word **LOVE** occur.
3. Then combine these numbers to make a 2-digit number and print it out.

---
~~~python
def calculate_love_score(name1, name2):
    combined_name = name1 + name2
    t_score = 0
    for letter in "true":
        t_score += combined_name.count(letter)
        
    l_score = 0
    for letter in "love":
        l_score += combined_name.count(letter)    
    
    final_score = int(str(t_score) + str(l_score))
    print(final_score)
calculate_love_score("Angela Yu", 'Jack Bauer')
