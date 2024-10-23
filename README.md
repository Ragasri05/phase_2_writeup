The Cryptic Dance 

![image](https://github.com/user-attachments/assets/82682a63-565e-4cfa-83ed-05519c369deb)


![image](https://github.com/user-attachments/assets/d0f9c0aa-eb28-48c3-afbe-3688daf0b426)

![image](https://github.com/user-attachments/assets/27c73c89-6da5-4d9c-9a39-415938da4083)

from the above image the decoded text is : ciphersarecool


Key code Mystique


<img width="562" alt="image" src="https://github.com/user-attachments/assets/ff16aa57-5e5b-4e3d-a702-aa8282ba0f51">


![image](https://github.com/user-attachments/assets/ed6af4d8-fb20-4304-8ade-23c4f56696da)

if we observe the keyboard, "a" is enclosed by qsz; n is enclosed by bhm; "d" is enclosed by sefc; "r" is enclosed by edft; "o" is enclosed by iklp; "i" is enclosed by ujko; "d" is enclosed by sefc; "i" is enclosed by ujko; "s" is enclosed by axdw; "f" is enclosed by drgv; "u" is enclosed by yhji; "n" is enclosed by bhjm.

so the decoded text is "androidisfun"



![image](https://github.com/user-attachments/assets/c50f21e0-b0fd-45b3-a066-995e0f813dab)

Steps to get the flag

Step   1: 

![image](https://github.com/user-attachments/assets/779b0eb4-f893-4a56-ab4f-f2d7326db3c6)

nikto: Scan web server for known vulnerabilities

-host: focuses it's scanning on a specific website or ip address.

give the ip address with port.

Step 2:

![image](https://github.com/user-attachments/assets/04e73000-d133-45b8-8132-883405f3dbaa)

dirb: DIRB IS a Web Content Scanner. It looks for  existing (and hidden) Web Objects.

then enter the URL

Step 3:

click on each directory (ctrl+click) and check.


![image](https://github.com/user-attachments/assets/0bf72127-221e-41d5-956f-7bce25c1b4db)

step 4:

go to flag.html.


![image](https://github.com/user-attachments/assets/0b2d1da5-14f7-4108-8d3a-177b74fc9794)

The Dragons Riddle 



![image](https://github.com/user-attachments/assets/9efb103a-d13b-4afa-a5bd-294efb0c66fe)

steps to get the flag

step 1:

![image](https://github.com/user-attachments/assets/bb4192e6-a800-4d15-a6c5-cce9c3920c99)

find the type of flag .

commands used : file

Step 2:

![image](https://github.com/user-attachments/assets/e2e4f8f4-1cb6-4ecd-90fd-da79d176b837)

found readable strings from the file 

commands used: strings 

step 3:

![Screenshot 2024-10-15 230027](https://github.com/user-attachments/assets/97b2e885-f0dd-413c-861a-32baacaac4fc)

these strings different from other text.

step 4:

decode the text.

the string can be decoded using base 64 decoding.

![image](https://github.com/user-attachments/assets/c78aa8b7-069a-4b11-a2f1-aa71ca388eae)

![image](https://github.com/user-attachments/assets/6d823818-3615-4ba3-b5e2-818643381bbd)

step 5 :

decode the octals using command : printf 

![image](https://github.com/user-attachments/assets/71362056-a4ad-4329-9cc6-660bd86f5dc9)

open the link.

![image](https://github.com/user-attachments/assets/32593653-285e-4e04-94f7-63729c48b85a)




ssh brute 


![image](https://github.com/user-attachments/assets/a8bea569-b30c-49a8-b6b6-ed52ee79e97d)


step 1: looking for password in rockyou.txt (it is inbuilt file in kali linux). 

commands used: hydra -l username -p /usr/share/wordlists/rockyou.txt.gz ssh://ipaddress:port

![image](https://github.com/user-attachments/assets/d8bfee3a-a654-48fb-a654-e96a2ac18037)

password is bubbles

step 2: login to the ip address.

commands used:  ssh username@ip -p port

![image](https://github.com/user-attachments/assets/9972bd50-90a2-47e0-88c6-8b13666f3063)

enter the password.

![image](https://github.com/user-attachments/assets/2798efa0-7379-45ed-9309-28f738418fc2)

step 3: list all the files

commands used: ls


![image](https://github.com/user-attachments/assets/1cef6c5d-456d-4669-aa67-a971f94828c2)


step 4: open the file 

commands used: cat filename


![image](https://github.com/user-attachments/assets/edff4e53-8008-404d-b76a-e444b43594ff)


John loves Hashes 

![image](https://github.com/user-attachments/assets/d74bc252-70b7-4122-8a92-36c6dffc1450)

step 1:
identify the Hashes.

![image](https://github.com/user-attachments/assets/fae5a045-8f21-47ef-b597-eed0aac119db)

using hashid tool we can identify the type of hash.

![image](https://github.com/user-attachments/assets/dbbb6f6f-ac02-46ce-a15f-dcdbbc51e464)

install hashid using "sudo apt install hashid"

1. ![image](https://github.com/user-attachments/assets/b10d31a1-5ee7-4981-b093-ca1e9c3ee4df)

2. ![image](https://github.com/user-attachments/assets/a4b3a292-2f30-4ed5-9086-ba0fe8cc7f9e)

3. ![image](https://github.com/user-attachments/assets/a4dc238e-6b30-404c-8f7f-2ebba4fb49ab)


4. ![image](https://github.com/user-attachments/assets/8d97fb80-0b79-4a9a-a3e3-69f70a4ab4ba)

5.  is bycrypt(since it starts with $2b$). mode is 3200 
step 2:

create a text file with each hash in separate line.

commands used : nano 

![image](https://github.com/user-attachments/assets/66c8fc2b-894d-468b-8ebf-cd07f8599ba8)


![image](https://github.com/user-attachments/assets/f9669861-9ef2-4660-84dd-0b0ca8b7ce50)


Step 3: 

install hashcat.

![image](https://github.com/user-attachments/assets/7547092f-d368-475a-9220-76f19fb5cb78)


use hashcat : Hashcat is a fast password recovery tool that helps break complex password hashes.

step 4:

know the mode of hash 

to get the mode use the command: "hashcat --help"

![image](https://github.com/user-attachments/assets/a6d4251c-eaae-4971-8b1e-5190fc022eaa)

![image](https://github.com/user-attachments/assets/df8c4e1b-da83-412b-800a-47dca181dc47)


![image](https://github.com/user-attachments/assets/5a8247f6-4a27-4be8-be6b-dcadbbb98661)


![image](https://github.com/user-attachments/assets/9c9b02a9-fd1e-4a2e-96d7-2f1f0f814124)


![image](https://github.com/user-attachments/assets/7e925abc-30e1-4a2d-9a1c-fbf5e1025b0e)


step 5: 

give the command : 

hashcat -m mode -a 0 hashes.txt /usr/share/wordlists/rockyou.txt.gz --show

![image](https://github.com/user-attachments/assets/3e21c7fa-01cc-4f9c-bf5a-c461a9a14896)


![image](https://github.com/user-attachments/assets/6654a475-5f3a-4e85-aed6-002ad54b9beb)


![image](https://github.com/user-attachments/assets/20012f2a-1d1e-4f7e-9cac-d0ed028aacf5)


![image](https://github.com/user-attachments/assets/30e5f8e0-2ec4-4673-a937-1b782d9a2c15)


![image](https://github.com/user-attachments/assets/837ab876-77f3-4063-b64a-b0dd34405e29)


note: removed the first hash from the hashes.txt file.

![image](https://github.com/user-attachments/assets/9168cf04-bcfd-44b2-a1f7-c9f4ae0af022)


![image](https://github.com/user-attachments/assets/3eb08399-5174-4e90-a912-e0c3cce4f437)


![image](https://github.com/user-attachments/assets/ccb8f499-3af9-43cf-b868-46795a1ca4d2)


![image](https://github.com/user-attachments/assets/3d09b740-135e-47e5-93b9-40866957ebe1)


![image](https://github.com/user-attachments/assets/8e46476f-6d14-42eb-8a1c-97397f33168f)































overly obfuscated

![image](https://github.com/user-attachments/assets/642e440e-de82-4578-9a9a-7d526ad8d104)

step 1: 

download the file and check for the type of file

![image](https://github.com/user-attachments/assets/d2413dfa-9196-4f18-be76-62ca6bcc9986)

since the text is ending with two equal signs , checking it for base64 

![image](https://github.com/user-attachments/assets/ced1d540-72c3-426f-849d-830459729d5c)

so the text base64 encoded text.

step 2: 

decode the text

command used : "base64 --decode inputfilename.txt > outputfilename.txt"

then open the file using : cat outputfilename.txt

![image](https://github.com/user-attachments/assets/c26f0c68-5123-474c-9baa-eaa6a91e0905)

reapeated this till i got the flag

![image](https://github.com/user-attachments/assets/bd59294f-eb99-4cd4-8c59-01cf2c822810)

.

.

![image](https://github.com/user-attachments/assets/db287ac3-e1b2-4dbd-bdec-4517ae3c03c6)



The open Book

![image](https://github.com/user-attachments/assets/2563d53d-2ba9-4782-90c0-231ba88b3278)


searched in google about Ethereum Sepolia

open this website

![image](https://github.com/user-attachments/assets/7815be16-fec4-4230-82eb-b1b319c79af1)

copy paste the etherium sepolia address in sepolia testnet explorer  

![image](https://github.com/user-attachments/assets/f18f8b15-782e-41f6-8df4-a6310b972b4d)


look for flag and open the transaction.

The flag is hidden here

<img width="978" alt="image" src="https://github.com/user-attachments/assets/1e3da3ad-1a1e-4399-978a-882eb0b30e4a">


<img width="683" alt="image" src="https://github.com/user-attachments/assets/1d524263-117a-49cc-b9f7-c2d52a773eea">

open the link

search for flag in these

![image](https://github.com/user-attachments/assets/6efdfcd4-6f0d-4f1a-96b8-23bbf4b4ac0b)

the flag is hidden here 
<img width="1007" alt="image" src="https://github.com/user-attachments/assets/8bc09e3f-4022-40e1-8fb9-1f4257c7df06">

click on show more
![image](https://github.com/user-attachments/assets/78bfae6d-9805-4111-9b9f-325913cc2729)

docode the text
![image](https://github.com/user-attachments/assets/1c042ee4-e463-4fb4-bcca-10b9dd6cd6da)


![image](https://github.com/user-attachments/assets/1bcda4da-7f50-402d-82e7-976a2237e80f)


































