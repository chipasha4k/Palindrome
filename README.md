# Palindrome
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
