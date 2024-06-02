def caesar_encrypt(message, shift):
    encrypted_message = ""
    for char in message:
        if char.isalpha():
            ascii_offset = 65 if char.isupper() else 97
            encrypted_char = chr((ord(char) - ascii_offset + shift) % 26 + ascii_offset)
            encrypted_message += encrypted_char
        else:
            encrypted_message += char
    return encrypted_message

def caesar_decrypt(encrypted_message, shift):
    decrypted_message = ""
    for char in encrypted_message:
        if char.isalpha():
            ascii_offset = 65 if char.isupper() else 97
            decrypted_char = chr((ord(char) - ascii_offset - shift) % 26 + ascii_offset)
            decrypted_message += decrypted_char
        else:
            decrypted_message += char
    return decrypted_message

def main():
    while True:
        action = input("Would you like to 'encrypt' or 'decrypt' (Type e or d or QUIT to quit): ")
        if action.lower() == 'e':
            message = input("Enter the message to encrypt: ")
            shift = int(input("Enter the shift value: "))
            encrypted_message = caesar_encrypt(message, shift)
            print("Encrypted message:", encrypted_message)
        elif action.lower() == 'd':
            encrypted_message = input("Enter the message to decrypt: ")
            shift = int(input("Enter the shift value: "))
            decrypted_message = caesar_decrypt(encrypted_message, shift)
            print("Decrypted message:", decrypted_message)
        elif action.upper() == 'QUIT':
            break
        else:
            print("Invalid input. Please try again.")

if __name__ == "__main__":
    main()
