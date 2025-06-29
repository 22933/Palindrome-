def is_palindrome(number):
    number_str = str(number)
    
    # Check if the number has exactly 12 digits
    if len(number_str) != 12:
        return False, "The number is not 12 digits long."
    
    # Check for palindrome
    if number_str == number_str[::-1]:
        return True, f"{number} is a 12-digit palindrome."
    else:
        return False, f"{number} is a 12-digit number but not a palindrome."

# Example usage
num = 123456654321
result, message = is_palindrome(num)
print(message)