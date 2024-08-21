# Password Cracking Using John the Ripper

## Objective

Performed a password cracking operation on a hashed password file using John the Ripper to demonstrate the effectiveness of brute force and dictionary attacks in a cybersecurity context.

### Skills Learned

- Hash Cracking: Leveraging John the Ripper to decrypt hashed passwords.
- Dictionary Attack: Using pre-defined wordlists to expedite the password cracking process.
- Brute Force Attack: Applying systematic guessing techniques to uncover complex passwords.
- Linux Command Line Proficiency: Executing and automating password cracking processes within the Kali Linux environment.

### Tools Used

- Kali Linux: As the operating system for running password-cracking operations.
- John the Ripper: For performing brute force and dictionary-based password cracking.
- Wordlists: To support dictionary attacks by providing a range of potential passwords.

### Outcome
This project successfully demonstrated the use of John the Ripper for cracking password hashes, providing insight into the vulnerabilities of weak passwords. It also highlighted key skills in hash cracking, attack methodologies, and command-line proficiency within a security-focused Linux environment.

## Steps

Create users for the project and give them weak passwords 

![Screenshot 2024-08-19 163117](https://github.com/user-attachments/assets/d208194a-b0ed-42f8-85ed-bf48be1c6eb6)

![Screenshot 2024-08-19 163225](https://github.com/user-attachments/assets/d3475530-a22d-482b-82d0-48dec3a9a2a0)

--------------------------------------------------------------------------------

Navigate to the shadow file and the passwd file to view the hash and file path of both of the test users and their password hash 

![Screenshot 2024-08-19 163225](https://github.com/user-attachments/assets/c010563a-6e9e-4972-abc9-702d93ff9a8c)

![Screenshot 2024-08-19 163245](https://github.com/user-attachments/assets/e3ad71e9-3a1e-4cc7-9823-8e802a2dd67e)

--------------------------------------------------------------------------------

Copy the shadow file (where hashes for passwords are stored) into a new file, in this case, text.txt.

![Screenshot 2024-08-19 163455](https://github.com/user-attachments/assets/b2fc464c-297a-40fa-8678-addd790ce704)

--------------------------------------------------------------------------------

Open the new file with all the hashes and filter out the hashes so that only the accounts we want to crack are in the new test.txt file 

![Screenshot 2024-08-19 163524](https://github.com/user-attachments/assets/aff03540-2dab-446f-96bf-4931bb9ce7dc)

![Screenshot 2024-08-19 163548](https://github.com/user-attachments/assets/ecd4ad54-d6d1-4e6d-b14f-393e4a91707b)

![Screenshot 2024-08-19 163608](https://github.com/user-attachments/assets/27f9b029-0b95-43c1-bd02-98ce8591c265)

--------------------------------------------------------------------------------

For this project, we are using the Rockyou word list, which was downloaded from a git repo; for the script, we are using John, which initiates the password crack, and then the path to the wordlist we will use.In this case, rock you. Then enter in the file fo the hashes we want to crack (text.txt) and finally the format which is how the hashes are encrypted (the type of encryption)

![Screenshot 2024-08-19 163651](https://github.com/user-attachments/assets/8ec0bd15-d333-40cc-901f-0a6d5b39cc3d)

--------------------------------------------------------------------------------

Allow it to run and wait for JTR to give us our passwords 

![Screenshot 2024-08-19 163737](https://github.com/user-attachments/assets/dd1b593b-6cb3-4bff-b236-7b32357143a1)

--------------------------------------------------------------------------------

We can use the (--show) command to view all of the cracked hashes

![Screenshot 2024-08-19 163910](https://github.com/user-attachments/assets/cd1820f7-9241-4292-b195-21d5c651192a)

--------------------------------------------------------------------------------












