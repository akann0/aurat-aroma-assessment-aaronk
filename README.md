# Aurat Aroma Tech Assessment - Aaron Kann

## Case Explanation
While there are a lot of possible use cases for a cognitive twin, 
the most interesting case to me would be an Emotional AI Therapist
that could provide mental health help to patients for minimal charge.  

While the ethics of such a product are debatable, especially with AI
still developing, a cognitive twin with estimated neurotransmitter levels
of each subject would be of great use to such a therapist. 
Knowing the estimated neurotransmitter levels of their online subject - 
and most importantly, what they lack relative to their career and personal goals - 
would help an AI therapist
improve the effectiveness of their advice by allowing them to use 
language in a way that is more impactful for their patients. 

## The Code
After completion of
[the form provided](https://sleepy-forest-18847-e830f43163a6.herokuapp.com/),
my code looks through the answers given for any possible hints at an olfactory profile.  
It uses gendered libraries to gather hints on gendered names in the name and email,
and seeks to match it with provided information on birth sex to build a base
neurotransmitter profile based on this information, as well as any hints 
as to the age of the user based on the name.  
After that, Natural Language Processing is used to take in inputs from various other
fields as well, using vectorized words to seek for hints of an olfactory profile from information based on
their career aspirations, workplace hindrances, and childhood nostalgia intertwined
with olfactory senses. 

The Data Analysis Code can be found [here](data_analysis.py)

## The Output
The form outputs, as an API would, a dictionary containing many different variables that might be of interest to the user.  In the sample case I provided, the olfactory information most useful to the data collector would be that of the 
neurotransmitting needs of the user. 
Notably, the Emotionally Regulating API might pull
- "dopamine_need"
- "gaba_need"
- "oxytocin_need"
- "serotonin_need"
- and finally, "glutamine_need",

which represent the neurotransmitters in which the user might be deficient or lacking.

## Notes for the Developers and Possible Places for Improvement
While this represents a step in the direction towards an olfactory profile,
there are places where this code could be improved before shipping a finished product.

A developer interested in refining this might consider

- reading up on scientific literature regarding neurotransmitter levels in order to more accurately calculate estimated deficiencies in females vs males, and age, and
include ethic origin in the calculations
- testing the vectorized NLP approach to see how effective it is in identifying neurotransmitter deficiencies
- use an NLP tool to identify parts of speech in the longer blocks of text, as removing filler words will most certainly improve the accuracy of the NLP approach
- use test data to idenitfy which prompts are most effective at identifying neurotransmitter deficiencies, in order to weight the averages provided

Thank you for your time! For any inquiries contact me at aaron@stevek.com