---
layout: essay
type: essay
title: Musings on spaces and braces
date: 2016-02-09
labels:
  - Coding Conventions
---
  I believe coding standards are an important concept for writing code. I think for the most 
part it improves readablity and therefore it is then easier to think about and maintain the 
code. One particular way I like to structure my code is to have code that is directly related 
to each other be clumped together with white space seperating it from other code. Another 
thing that I like do to, that I notice most people don’t, is set my curly braces on a new line.

For example:  
   
if (some condtion)   
{    
    do something   
}    
else      
{    
    do something else   
}    
    
Now compare that to:    
    
if (some condtion) {        
    do something   
} else {    
    do something else    
}     
    
The second option drives me insane. I feel like I have to search for the curly braces and the 
else statement. What if there is a missing brace? It is so much easier to find a missing brace 
in the first option. Smart use of use of white space with proper indention makes everything so 
much easier to understand. This is one reason I think python makes a great language to learn 
for someone’s first time, because it forces indention for readability.
	
  Although I think coding standards improve readability, there are some that make it worse. The 
first time I encountered Win32 programming I found some very strange names coming from Microsoft.
      
Take this for example: LPCTSTR lpString.     
    
Obviously it’s some sort of string but what is ‘lp’ in 
the variable name? Or even worse what is ‘LPCT’? If you follow the trail far enough on MSDN, you 
will eventually find it is just a char pointer. This type of code is all over the place once you 
include the Windows header and it’s an eyesore to say the least. I had to constantly look up 
these little acronyms to make sure I understood what I was working with. This notation is called 
Hungarian notation and it should be condemned to lowest depths of hell.
	
