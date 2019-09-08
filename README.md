# node-markov
Given a text input, will create a Markov chain.
This is a script that when passed in a file or a url, it will take the text and convert it into a Markov chain.
If a URL is passed in, it will strip out the html so only the text will remain.
A Markov chain takes the text and attempts to "smartly" rearrange the words creating a new text.
The new text is created by linking together words that were originally next to eachother, adding readability.


Setup:
node makeText.js <file or url> <file path or url> 
example:
  node makeText.js url www.github.com bigram
  node makeText.js file ../eggs.txt
 
Eggs.txt is sample text for testing purposes. 
  
You can also optionally add "bigram" at the end as a final argument. A bigram chain links together two words at a time,
making the text more readable but less random. 

Testing:
npm test

