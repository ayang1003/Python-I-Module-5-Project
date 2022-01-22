# Python-I-Module-5-Project
This project mainly focuses on slicing, for loops, and if statements. The first part prints the variable "longWord" backwards, prints the first and last character of said variable, and prints how many vowels are in it. The second part prints a user-given phrase in reverse and replaces the letters "a", "e", "i", and "o" in said phrase with "@", "#", "%", and "*" respectably in order to create a sort of coded message.

# Part 1
longWord = "supercalifragilisticexpialidocious"
print(longWord[::-1])
print(longWord[0] + longWord[-1])
i = 0
while i < len(longWord):
    print(longWord[i:i + 8])
    i += 8
count = 0
for letters in range(len(longWord)):
    if "a" in longWord[letters]:
        count += 1
    elif "e" in longWord[letters]:
        count += 1
    elif "i" in longWord[letters]:
        count += 1
    elif "o" in longWord[letters]:
        count += 1
    elif "u" in longWord[letters]:
        count += 1
print(count)

# Part 2
userWord = input("Enter the secret message: ")
userWord = userWord[::-1]
userWord2 = userWord.lower()
newWord = ""
for letters in range(len(userWord2)):
    if "a" in userWord2[letters]:
        newWord += "@"
    elif "e" in userWord2[letters]:
        newWord += "#"
    elif "i" in userWord2[letters]:
        newWord += "%"
    elif "o" in userWord2[letters]:
        newWord += "*"
    else:
        newWord += (userWord[letters])
print(newWord)
