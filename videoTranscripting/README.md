# NLPYouTube
 Natural language text chat bot attempt using videos from TEDx

 ## Setting Up
 Download the whole directory and install the needed modules which all in the first cell, I deleted the raw files to save space and clutter, running the cells will automatically get the back.

 ## Objective
 This is my first attempt at Natural language processing where I wanted to create something out of information not readily available.

 ### Workings
 The programs utilizes selenium to scrape (n)-number of href elements and returns a list of video links\
 downloaded via pytube,\
 converted to .wav using ffmpeg python wrapper ffmpy,\
 split into user defined pieces,\
 the splitting can either be by duration of silence or by a tixed time length,\
 I prefer the latter to have uniformity in size and line duration but is a lesser reliable way for machine training.\
 These aplit up audio cables are transcribed using google voice recognition and are appended to a list which in the end becomes the training corpus.\
 The model is a copy-paste from the google tensorflow Zero to Hero NLP series since I have no knowledge of half  the things in this part.

 #### This was done purely for fun and testing purposes and needs to be revisited for improvement on results,
 #### the transcribing is inadequate as no key has been used which unlocks finer tunable features of goolges' voice recoginizer,
 #### Tensorflow model is not optimized at all,
 #### Transcribing takes much longer than I would like.
 