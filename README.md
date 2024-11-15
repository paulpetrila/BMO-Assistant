# BMO Assitant 
A voice assistant with a good wake-on-word engine and great support for interacting with things around the house.

  * [Minimum requirements for my Bachelor's Thesis](#minimum-requirements-for-my-bachelors-thesis)
  * [Greater Vision <sub><sup>(extreme scope creeping)</sub></sup>](#greater-vision--sub--sup--extreme-scope-creeping---sub---sup-)
  * [Resources](#resources)
    + [Articles and scientific research that I examined while making the project](#articles-and-scientific-research-that-i-examined-while-making-the-project)
    + [Similar projects](#similar-projects)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>



## Minimum requirements for my Bachelor's Thesis
A small proof of concept that could be extended according to my needs and a project that I can use to test my theories about how everything is going to turn out.
- [ ] Train a specific wake on word net to achieve
    > Motivation: false positive rate from outside sources (sounds coming from the TV or casual conversation)
- [ ] Use whisper to transcribe English or Romanian speech into text 
    > Motivation: Most projects don't enable Romanian language as an input source 
- [ ] Train an NLP (BERT) to recognize commands from the text generated from the OpenAI Whisper speech2text
- [ ] Train BMO voice on some robot dataset/ actual Adventure Time footage
- [ ] Command to send a file to octoprint/klipper
- [ ] Generate a new background based on classic art or a certain classic artist
- [ ] Convert the models to the ONNX runtime so that they run faster and on any platform




Once I have the software ready, I can get into printing the case that Allie used in her [BMOctoprint](https://github.com/katzcreates/BMOctoprint) project.
Thank you, [Allie](https://github.com/katzcreates)! 

And after that I'm going to add other triggers, and thanks to Whisper, I only need to retrain the NLP Layer.
- [ ] Command to set an alarm for a certain time
- [ ] Command for a timer
- [ ] Command to close lights



## Greater Vision <sub><sup>(extreme scope creeping)</sub></sup> 

Multiple agents(personas) that could control different things around your house or help you with different tasks. Agents can be shared and their skills retrained on your on needs. Some skills might need a sudo permission in order to get called, the agent says something like "I can't do that, sudo required" and in order to execute it, the owner needs to scan his face.

It would be nice to find a way to teach agents new skills without going into the config files. But for that, I'd need to implement some sort of driver over things like Home Assistant or to surf websites for them, like going to a website and inputting what they said, like a Robot Process Automation client. "Go to website X and search for Y in the Z field".

Some personas that I came up with and I'm trying to implement: 
1. Monoclus - A DnD sidekick that could help you by pre-programming certain sequences, sounds, combat/ ambient playlists or characters. Should be able to be asked for hints or act as a bar tender with the party. Sudo would be required to edit the shop, the inventory of players, change the TTRPG it's set to etc.
2. BMO - should play music, search the internet, keep track of a grocery list etc

## Resources
### Articles and scientific research that I examined while making the project 
- [Reproducible code article](https://www.coronawhy.org/presentations/reproducible-reusable-code-in-python)


### Similar projects
Some of these are actively maintained, some aren't. The scope of my project is to make something similar, but with less false positives, as this is the most common complaint from the users.

- [Open Interpreter](https://www.openinterpreter.com/)
- [Rhasspy](https://community.rhasspy.org/)
- [Open Voice OS](https://www.openvoiceos.org/)
