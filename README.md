# quizbowl_stuff

I wanted to figure out what the most common tossup categories were in order to figure out which areas to spend more of my time on, and so I decided to scan a few packets to figure that out. I ended up doing
it for 240 packets and about 5000 questions.

I collected the links for those 240 pdfs from the quizbowl site and they cover tournaments from 2021-2023. The pdf was saved and then scanned using the pypdf library - this naturally consumes the most amount of time while running the code. The text is then scanned
for matches of the form \<some text\> as that is how the categories are usually typed in the packets. All of the categories and their counts are then stored in a dictionary.

The next step is cleaning the data since there is no standard way of listing the categories and pretty often we find the name of the authors listed right beside the category. This step consumed the most time for me to write.
We can then plot this data to see the results.

The graph might show that mythology is the most common category but I'm cheating here a little bit - all the literature(European, American etc), history(American, World etc) and science(Physics, Bio etc) categories are split
up, and if we add those up the picture becomes a lot less surprising : 1011 in total for both Literature and History, and 1006 for Science

It was only after spending hours on this that I realised that the entire exercise might be futile. It was only at this time that it occurred to me that maybe it might to a good idea to check if there was some forum or website
where this distribution was clearly specified. Of course, it was.

Nevertheless, I hope you have fun going through it.
