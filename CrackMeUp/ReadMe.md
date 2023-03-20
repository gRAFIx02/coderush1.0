# Problem Statement
Aashnan thought his secret wont be compromised. Being the clever guy he was he even kept his secret hidden using some tricks even if it gets leaked. Surely it cant be cracked, right?

flag format: coderush{fl4g}

# Solution
This is a simple steg problem. To solve this, you will need a steg tool like `steghide`. Before using steg, you will see a file with a couple of hash values. You can crack them from [here](https://crackstation.net/).
Once you crack the hashes, you will get some valid and invalid results. One of the valid results is the password for the steg operation that you will be doing on the `logo.jpg`.

![Screenshot 2023-03-20 104913](https://user-images.githubusercontent.com/71190713/226250832-6430c934-d88b-477a-b536-0788ceabb449.png)

Now, go to terminal and use the command `steghide extract -sf logo.jpg`. You will be asked to enter a password. Use the cracked results from the hashes one by one till you get the correct password. In this case, the correct password was `strangerthings`.

![Screenshot 2023-03-20 105034](https://user-images.githubusercontent.com/71190713/226251160-ab1fda34-e3d6-449c-81c1-0d73e3c8a4fc.png)


Correct password will give you a flag.txt file. Inside the file, you will get the flag.
## The flag
coderush{b3c4r3fu11_4b0u7_7h3_h45h_y0u_u53}

**__h4ppY h4aCk1Ng__**
