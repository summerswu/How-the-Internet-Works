# Western Founders Network Educational - How the Internet Works 

image[https://cdn-images-1.medium.com/max/1200/1*zQI-4a89t-t8bEfcztNTiw.png]

## Introduction 

In this section we looking at the evolution in the way we communicate

1. Postal Protocols in Ancient China - Yam Routes Established Across the nation: At it's peak there were 1785 established post offices and 300,000 horses distributed around these offcies. Peak travel time can reach around 400km a day - equal to back and forth trip from London to Toronto

2. Telegraph - Telegraphy is not what would be commonly considered as a "Telegraph"
      - Electrical Telegraph - Five Needle Telegraph vs. Morse Key - employ the use of electro magents - marvelous piece of engineering
      
3. First look at Internet Protocol Suite - 7 layers of Protocal Stack in the ideal Open System Interconnect Reference Model(meant for teaching and demonstratuion hence the name reference - developed around 1977)

*END OF INTRODUCTION*

### INTERLUDE-Basic Computer Logic 

In order to understand the complexity of the computers and network protocols of today, we need to first take a look at binary logic and the simplest logic gates that constructs the Arithemitic Logic Units inside the computer 

https://www.youtube.com/watch?v=gI-qXk7XojA : Crash Course - Boolean Algebra & Logic Gates

Understanding this at a transistor level is a different story and will not be discussed here - second || third year Software/Electrical/Computer Engineer stuff  

  http://nandgame.com/ : Cool Game that lets you construct a ALU units using the simplest logic
  
  https://www.nand2tetris.org/ : if you have a little more time you can play this, building a whole OS from the ground up
 
  https://store.steampowered.com/app/370360/TIS100/ : Repairing an old broken computer, great way to practice logical thinking and learn a thing or two about computer networking 
      
## Connecting the Dots

Throught out this workshop, there will be a lot of abstractions given the complexity and scale of the subject discussed, the key here is to gain a high level understanding, don't fret over small techincal details

The gist of it is - everything on the internet is a computer, including a server 

https://www.lifewire.com/servers-in-computer-networking-817380 

https://www.webopedia.com/Computer_Science/Client_Server_Computing - both links contain excellent laymen explanation 

There are many different types of servers and they each function differently, a lot of servers today are running multiple kernels, load balancers, and shells as well as read and write databases all on the same machine. If we ever get to do a cloud computing work shop we can dive deeper into this subject 

#### Live-Drawing Segment 1
Now we switch over to the drawing pad to illustrate the puzzle and iteration problem solving that went into solving the puzzle

- The story of Brad, Chad and Becky and how they talk to each other
- Brad is trying to talk to Becky but he can not reach her - so he tries to talk to her through Chad 
- PROBLEM!: Their communication is not secured! 

[The Drawings will be updated onto the document]

### INTERLUDE-Cryptography 101 

The Caesar Cipher is one the first ciphers in the world - used by Julius Caesars messengers to transport intelligence message during war
 
http://practicalcryptography.com/ciphers/caesar-cipher/  - Introduction and Demo

https://demonstrations.wolfram.com/SimpleCaesarCipher/ - Wolfram Demo of the Cipher 

Two Problems with this Code: 
      1. Becky have to know the key before hand 
      2. The encryption is over simplistic
      
Introducing - Public Private Key Encryption 

http://cobweb.cs.uga.edu/~dme/csci6300/Encryption/Crypto.html - high leve implementation and demonstration, does not explain the actual mechanism behind this method of encryption 

(Rivest–Shamir–Adleman) System of Encryption - generate keys - http://www.csfieldguide.org.nz/en/interactives/rsa-key-generator/index.html

Again this is all abstraction, we do not have the mathmatical tool set or time to deep dive into the math behind this topic

#### Live-Drawing Segment 2

Now Brad have a secured way of communication through Chad to Becky, we will formalize this abstraction

Brad = End-User 
Chad = Router 
Becky = Server 

PROBLEM with our abstraction - There are some many more computers in the network

SOLUTION - many more computers, routers, and servers are interconnected(computers make request, router direction request to designated server, server hands back response, response travel back to comuputers through routers) - do you see any similarities? 

PROBLEM - how does information need to know where to go? 

SOLUTION - DHCP servers, IPv4 Address Protocal 

PROBLEM - Too many devices!

SOLUTION - IPv6 Address Protocal 

PROBLEM - What if we would like to switch servers? Plus, it is so hard to memorize all the 6 byte addresses for each website. 

SOUTION - DNS Systems and Servers(each must register a unique domain)

Quiz: What does the www stand for?

**USING ROUTERS LIKE THE ANCIENT CHINESE POST OFFICE WE ARE ALLOWED TO DIRECT, USING FIBRE OPTICS/OTHER PHYSICAL COMMUNICATIONS WE ARE ALLOWED TO TRANPORT DATA AT A EXTREMELY HIGH SPEED, AND USING LOGIC UNITS OF THE COMPUTER WE CAN INTERPRET THESE MESSAGES EASITLY**

## Who owns all of these routers and who owns all the servers in the world?  

Demonstration Time: 

Open up command prompt - 

Ping: sends four packets to a server and ask for a response 

NsLookup: look up the ip address of a particular website or look up the DNS server itself 

most interesting one: TRACERT checks over maximum of thirty hops where you request got routed to and reports back

## How exactly are information handled? 

The envelop excersie - again, this is just an abstraction - Introduction to TCP/IP model packets

TCP/IP(Sequence Number) - ensure proper communication in the right sequence and reassembly, can make request to gurantee delivery 

UDP - what if you don't want to ensure gurantee delievery? when would you want to make such a request

Going onto HTTPS


## Book Lists




       
