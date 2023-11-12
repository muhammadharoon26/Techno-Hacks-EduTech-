# Password Cracking through Hashcat and John the Ripper
Cracking a simple password like "password123" using tools like Hashcat and John the Ripper.

# Procedure
1.  Convert the password ("password123" in this case) to hash form. (MD5 is used in this task)
2.  Store the hash in a file.
3.  Install wordlists on kali by entering the command:

        sudo apt install wordlists

# Hashcat
->  Navigate to the location of file which contains the hash.  
->  Enter this command:

        sudo hashcat -a 0 -m 0 <name_of_file_in_which_hash_is_stored> /usr/share/wordlists/rockyou.txt

# John the Ripper
->Type:

    wordlists

->  Enter this command:

    john  --format=Raw-MD5  --wordlist=/usr/share/wordlists/rockyou.txt <location_of_file_in_which_hash_is_stored>

