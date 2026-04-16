PALINDROME
WORK FLOW
1.	Start
2.	Enter a word
3.	Change the word to lower case
4.	Reverse the word
5.	Compare the original word with the reverse word
6.	If they are the same, display “Palindrome”
7.	If they are not the same, display “Not a Palindrome”
8.	End



PSEUDO CODE
BEGIN
	PRINT “Enter a word”
	INPUT word

	SET word = convert word to lowercase
	SET reversed_word = reverse of word

	IF word == reversed_word THEN
		PRINT “The word is a Palindrome”
	ELSE
		PRINT “The word is NOT a Palindrome”
	END IF
END




PYTHON CODE
def check_palindrome():
    print("Palindrome Checker")
    word = input("Enter a word: ")
    # Step 1: Normalize
    normalized_word = word.lower()
    print(f"\nStep 1: Convert to lowercase → {normalized_word}")
    # Step 2: Reverse
    reversed_word = normalized_word[::-1]
    print(f"Step 2: Reverse the word → {reversed_word}")
    # Step 3: Compare
    print(f"Step 3: Compare '{normalized_word}' with '{reversed_word}'")
    if normalized_word == reversed_word:
        print("\nResult: ✅ It IS a palindrome!")
    else:
        print("\nResult: ❌ It is NOT a palindrome.")
# Run the program
check_palindrome()
