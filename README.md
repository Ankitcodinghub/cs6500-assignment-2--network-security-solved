# cs6500-assignment-2--network-security-solved
**TO GET THIS SOLUTION VISIT:** [CS6500 Assignment 2- Network Security Solved](https://www.ankitcodinghub.com/product/cs6500-network-security-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;116524&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS6500 Assignment 2- Network Security Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
1 Project description

The objective of this project is to implement the various components of a security-enhanced EMAIL system similar to PGP (Pretty Good Privacy) and GnuPG which is based on the OpenPGP standard. The cryptographic libraries from:

• OpenSSL (www.openssl.org) (OR)

• Java JCA (https://docs.oracle.com/javase/7/docs/technotes/guides/security/crypto/ CryptoSpec.html) (OR)

• Python (https://pypi.org/project/cryptography) can be used

1.1 Encrypted Email

The task is: Given an email message from User A to User B, message digest algorithm, encryption algorithm and the public/private key pairs of users, generate a security-enhanced output message that will handle: (a) Confidentiality ONLY, (b) Authentication/Integrity ONLY and (c) Authentication/Integrity and Confidentiality. We will assume that for a given set of users, the corresponding public/private key pair is locally available. In reality, the public key information for each user is available from some keyserver and the private key is held securely by each user. For this project, we will assume that Triple-key 3DES, and AES are available. We will assume that only CBC mode is used. The encryption steps are explained in detail in Stallings’ textbook. In order to achieve the different levels of security/privacy, the following mechanisms are used:

Confidentiality ONLY (CONF):

Sender: The email message is encrypted with a randomly generated secret message key (or session key) using a symmetric block cipher algorithm. The message key is encrypted using the receiver’s public key and pre-pended to the message. The [encrypted key, message] is then written into a file that can be sent using traditional email. In essence, given input text M from user A to user B, the transmitted message C is:

C = [EKUb(Ks,IVs)||EKencralgs (M)]

where Ks is the session key (and any needed initialization vector, IVs) and EKUb is the receiver’s RSA public key. Receiver: The receiver uses its private key to decrypt the secret message key from the message file. This secret key is then fed to the decryption algorithm on the remainder of the message file to extract the plain-text message.

Authentication/Integrity ONLY (AUIN):

Sender: A message digest or hash of the given plain-text message is generated. The digest/hash is then encrypted using the sender’s private key. The [encrypted hash, message] is then written into a file that can be sent using traditional email. In essence, given input text M from user A to user B, the transmitted message C is:

C = [EKRa(Hhashlog(M))||M]

where EKRa is the sender’s RSA private key. Receiver: The receiver reads the encrypted hash from the message file and decrypts using the sender’s public key to generate the hash. The digest/hash of the remainder of the message file is computed and compared to the decrypted hash. If they match, success is declared.

Confidentiality and Authentication/Integrity (COAI): Sender: A message digest or hash of the given plaintext message is generated. The digest/hash is then encrypted using the sender’s private key. The [encrypted hash, message] is then encrypted with a randomly generated secret message key (or session key) using a symmetric block cipher algorithm. The message key is encrypted using the receiver’s public key and pre-pended to the message. The [encrypted key, encrypted hash, message] is then written into a file that can be sent using traditional email. In essence, given input text M from user A to user B, the transmitted message C is:

where Ks is the session key (and any needed initialization vector, IVs), Kh is the hashing key (of length equal to the hashing algorithm’s block size), EKRa is sender’s RSA private key and EKUb is receiver’s RSA public key. Receiver: The receiver performs the reverse operation to verify the sender, integrity and to extract the plain-text message.

1.2 User Interface

The following are the necessary commands:

• ./lab2 CreateKeys UserNameListFile RSAKeySize

The UserNameListFile will contain a set of users, one per line. RSAKeySize is either 1024 or 2048. For each user, randomly generate an RSA key pair and store private key and public key in user priv keylen.txt and user pub keylen.txt respectively; where keylen is either 1024 or 2048.

• ./lab2 CreateMail SecType Sender Receiver EmailInputFile EmailOutputFile DigestAlg EncryAlg RSAKey-

Size

SecType: CONF, AUIN, COAI are three possible string values for the three cases listed earlier.

Sender/Receiver are sender and recipient of this message.

EmailInputFile contains the input plain-text file (in ASCII format)

EmailOutputFile contains the output of the encryption algorithms (in binary format)

DigestAlg is one of: sha512, sha3-512

EncryAlg is one of: des-ede3-cbc, aes-256-cbc

• ./lab2 ReadMail SecType Sender Receiver SecureInputFile PlainTextOutputFile DigestAlg EncryAlg Similar to above.

1.3 Output File Format:

CONF: Line 1: Encrypted Secret Key

Line 2 onwards: Encrypted Data

AUIN: Line 1: Encrypted Hash/Digest Line 2 onwards: Plaintext Data

COAI: Line 1: Encrypted Secret Key

Line 2: Encrypted [Hash/Digest+MessageData]

2 Starting Point

2.1 System Calls

At the least, the following system calls will be required . On Linux, man command or info command will provide you with relevant information. You can run ’man evp’, ’man rsa’, ’man pem’ for lots of additional information. You should know or learn how to read function interface descriptions from man pages and use them correctly.

Note: By default, the crypto functions produce binary output. You must choose base64 encoded output format.

3 Sample Session

Assume that you have created the files lab3.c and the corresponding executables in your LAB2 directory

% cd LAB2 % make lab2

…

% pico Usernames.txt

… file will contain a set of 10-15 users

% ./lab2 CreateKeys Usernames.txt 2048

% ls -l * priv.txt * pub.txt

% pico Mail-sample.txt

… file will contain input text message.

% ./lab2 CreateMail COAI alice bob Mail-sample.txt Mail-out.txt sha512 aes-256-cbc 2048 .. Encrypted File is created.

% ./lab2 ReadMail COAI alice bob Mail-out.txt Mail-decrypt.txt sha512 aes-256-cbc 2048

.. Decryption operation

% diff Mail-sample.txt Mail-decrypt.txt .. Any differences?

4 What to Submit

Name your project directory as LAB2 (Note: ALL UPPERCASE) Once you are ready to submit, change directory to the directory above LAB2, and tar all files in the directory with the command:

tar czf Lab2-RollNo.tgz LAB2

Then, submit it online on Moodle. The directory should contain the following files:

• Source Files

• Makefile Typing command ‘make’ at the UNIX command prompt, should generate all the required executables.

• A Script file obtained by running UNIX command script which will record the way you have finally tested your program

• a README file containing instructions to compile, run and test your program. The README should document known error cases and weaknesses with the program.

5 Help

2. . Ask questions EARLY. Do not wait until the week before. This project is quite time-consuming.

3. Implement the solutions, step by step. Trying to write the entire program in one shot, and compiling the program will lead to frustration, more than anything else. For example, implement the message digest first, then try encryption with secret key, then try encryption with public/private key, etc.

6 Grading

• CONF: 30 points

• AUIN: 30 points

• COAI: 40 points

No README/COMMENTS: -5 points; No Script File: -10 points; Incomplete Compilation: -10 points
