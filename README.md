# Cover Capture
The goal of this project, is to create a Raspberry Pi based intrument recording set up. I will start with drums, and branch out from there. In the end, you will be able to choose any common instrument, and create a cover of whatever song you want.

# Design
The Raspberry Pi will be connected to the internet, as well as a series of several mics, which will be placed on the various drums on the drum set. The Pi will also act as a web server, so to access the interface, you would get on your laptop or desktop and access the pi locally. This way, you plug the Pi in, put the mics on the drums, and get on the local website and boom your done. There would be a shared database, as well as a local database for each user. So any cover songs that have been uploaded already by other users, would be available to everyone, unless they set a private flag on that track. 

A cover track would be any song that has the desired track removed. For example, a drum cover track would be a track with no drums. Otherwise known as 'minus drums' tracks. 

# Use Cases
## Creating a cover
To create a new cover, the user would need to either search for an existing cover track, or upload one that they found online. In the event that they upload a cover track, it would then ask them to match that track with a spotify track in order to learn more about the file they uploaded. Once they have matched the song, it would then upload the information to the shared server/database, as well as theirs locally. Next, the user would see a music playing interface where they can click to record a new track. When they click record, it would wait a few seconds to give them time to prepare, and then as most cover tracks do, it would have an 8 beat count down so they know when to play. When the songs starts playing, the Raspberry Pi also starts recording the mics. When the song is over, the Pi stops recording, and it prepares the result by combining the different mic tracks into one file. The user would then see the option (on the web interface) to listen to the result, upload the result to the internet, or delete the result and try again. 

# Clarification
In my head, this makes sense, but in case I did a bad job of explaining it, here is some clarification: 

There will be a live server with a database, that is accessible from the internet. Users can view other users uploaded covers, create profiles, etc. 

There will also be a raspberry pi, that creates a local web server. This would be necessary, because the live server would not be able to access the mics directly (or as easily). 

The user connects all the mics to the Pi, and puts them on the drums. This shouldn't be too hard, since I think they would be usb mics. There would be an interface on the local pi's website that allows them to specify which mic is on which drum. This information would be saved and editable.

The user then would select a song, either one that another user uploaded, or one that they upload. They would then record it and upload it. 

# Packaged Result
In the event that we sell this to other people instead of just for personal use, here is what I would hope to create:

A Linux kernel that would automatically create a local database, website, and connect to the live database/website as well. The user would only have to flash the kernel to a Raspberry Pi, and plug it in. The user would then only need to plug the mics in and go to the website to start recording. 



# Add Ons
Video!

