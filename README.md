# Enigma
An online Enigma Machine simulator for encrypting text. It is based on the functionality of the Enigma hardware encryption machine used during WWII.
  This web page recreates the functionality of the Enigma ecryption machine that was invented for commercial use,
but later used by the German military in World War 2.   The device used a constantly changing set of electrical circuit
pathways to take letters A-Z and numbers 0-9 and encode them to an encrypted cypher text.  This constantly changing circuit
allowed for much greater security than a simple substitution cypher. 
   In order for the recipients of the encoded messages to translate them back to plain text, they had to have 2 things. The first was 
their own Enigma machine, and the second was the configuration that the encoding machinhe used when the message was encrypted.
An Enigma machine used rotating cylinders that had 26 positions they could start from. Each time a character was pressed and encrypted 
their would be an advancing of the cylinders position that changed the electrical circuit paths.   Typically the machine used any three of a set f five cyliners. The three cyliders advanced at different rates much like the hour, minute and second hands of a watch. 
    The fast cylider rotated once every 26 character presses, at the 27th character the medium speed (middle) cylinder advanced one position, nd similarly when the middle cylinder made a full rotation the slow cylinder advanced one position.Because order matters we use P(n,r) {P(5,3)=5!/(5-3)! = 120/2 = 60} to determine the number of permutations we can select and arrange 3 cylinders from a set of 5. This gives us 60 ways.  Each of the 60 ways has 26 possible positions so we take 60 to the power of 78 (26 letters x 3 cylinders)
and arrive at 2.333034e+110 total ways that the Enigma machine can be configured.
    All of these possible ways for the machine to be configured were the result of choosing 3 cylinders from a set of 5 and then
choosing the orientation of each of the cylinders in 26 ways. Each configuration changed a physical circuit pathway that resulted in 
the lighting of a letter or number when a character was pressed on the machines keyboard. This lighed character was the cypher text and with he same circiut pathway when the cypher text character was pressed, it lit up the plain-text character enabling the decryption of the message.
     In this program arrays and pointers will be used to represent the cylinders and starting positions. The user interface uses drop-own
menus for the user to select the the cylinders and their starting positions.  In order to send an ecrypted message to someone, the recipient of the message only needs the cypher-text and the configuration settings that were used when the plain-text was encrypted.  
