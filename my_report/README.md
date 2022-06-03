# Lesson: Interaction Design

### First and Last Name: Gelena-Ilektra Kouletsi
### University Registration Number: dpsd19139
### GitHub Personal Profile: https://github.com/Kuletsi
### Augmented Reality Personal Repository: https://github.com/Kuletsi/Augmented-Reality

# Introduction

# Summary


# 1st Deliverable
The IDE I used for editing the code was Visual Studio Code. I did the deliverable entirely on my laptop so I set up the locahost:8000 by following the instructions on <a href="https://developer.mozilla.org/en-US/docs/Learn/Common_questions/set_up_a_local_testing_server"> How do you set up a local testing server? </a>.  I also downloaded GitHub Desktop but I didn't find it very useful, so I used the browser version. <br>
I linked the application in my respiratory at the lab. <br>
### The first Deliverable consisted of 3 tasks. <br>
The <b> first task </b> was adding two primitive shapes (a cylinder and a sphere). The code for the box was already given in the code so I copied and pasted it twice, and changed the "primitive: box;" to "primitive: sphere;" and primitive "primitive: cylinder;" accordingly. I also changed the ids. Then, I changed the colors of all three shapes (I found the hex codes online by googling "hex codes") and also their coordinates (their "position") so they wouldn't overlap. Lastly I arranged the height the width and the depth. (I made them quite big so the marker has to be a bit further away from the screen for all three to be visible).<br> <br>
The <b>second task</b> was adding snow to the scene. I found the code from A-frame school, <a href="https://www.npmjs.com/package/aframe-particle-system-component" > Α-Frame particle system component</a> as it was given to us in the task description. I copy pasted the code, and made the snow baby pink (I also just googled it). I tried putting the a-entity both inside the a-marker and outside and found that outside works better, so I left it there. <br> <br> 
For the <b> third task</b>, at first I found the code from the link that was give to us ( <a href="https://www.npmjs.com/package/aframe-speech-command-component" > Α-Frame speech command component</a> ). I combined the examples that were given to us in the link and I also looked at the public examples that were linked in the discussions (<a href= "https://github.com/lmalave/aframe-speech-command-component/tree/master/examples"> Public examples of the speech command </a>). <br>


# 2nd Deliverable
### The second deliverable consisted of 3 tasks. <br>
The **first task** was making a custom marker which when read displays an image and text. I made a square with my registry number written on it in photoshop and I uploaded it in <a href="https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html"> Custom marker generator </a>. Then I added it to my code and used one of the objects from the previous deliverable to test if it was working. It took some back and forth trying different fonts and sizes, but also bigger borders in the generator to get it to recognize my marker. After that I made the markers for Hydrogen and for Oxygen (since I was accustomed with the site) for later usage. <br> After that I tried to insert my text (my name). At first I did it with another tag (I think I somehow did it with _a-entity_, but it was 3 weeks ago and I honestly don't remember) but then I found _a-text_ and it behaved much better so I kept that. The text appeared flat when i first put it in, so I rotated it on the x axis. I did the same with the the image I chose. Later I also added a png image of a heart and I combined the three elements so they could all be visible (by editing their positions). Furthermore I changed the font of the a-text and the color. <br> <br> 
The **second task** was displaying 3D animations of the Hydrogen and the Oxygen atoms, by reading custom markers. I had made the markers previously. I made the 3D animations using blender and following a youtube video <a href="https://www.youtube.com/watch?v=kVBUzAnBcck&ab_channel=NEYOVA"> a youtube video </a>. I added colors and letters, and also played a bit with the texture and animation, which I learned how to do from various sources, by googling my queries. I tried various formats and ways of exporting (as a video, as a gif etc) but then I found I that the format needed was gltf . I exported it as a gltf by following  <a href="https://www.youtube.com/watch?v=p7OPRoT6FkY&ab_channel=DesignerHacks"> youtube videos </a> again and  <a href="https://blender.stackexchange.com/questions/120385/how-do-you-export-gltf-from-blender"> googling </a>. I put the gltf model inside my assets folder and inserted it in my code using the _a-entity gltf-model_ tag. The animation I did inside blender was not showing (I suppose I didn't export it correctly) but I animated it inside the code using the _animation-rotate_ component and making it run on a loop. I also tried fixing the position of the gltf models from the properties of the component so they would be parallel to the table when I used my phone to run the code but I had trouble doing so. <br> <br> 
The **third task** was showing a third animation displaying a water molecule when 3 markers (2 hydrgen and 1 oxygen) get in close proximity. At first I had trouble procesing the code from the examples I found online. After a lot of searching and also by reading the discussion under the second task in the repository (as well as looking at other codes) I didn't manage to make it work, even though I understand the logic behind the code. I have included the code that I tried to use, although it doesn't work. 




# 3rd Deliverable 
The **first task** was adding a 3D model of a place of interest and editing the coordinates in the properties of the a-entity accordingly. My first place of interest was Petra, in Jordan (which was also one of the 7 wonders) but I didn't have much luck finding a suitable 3D model on sketchfab. Then I decided to use  <a href="https://sketchfab.com/3d-models/fontaine-de-lobservatoire-paris-2fd367e20a32409b9e85a812b09f152c"> a 3D model of a parisian fountain called _Fontaine de l'observatoire_ </a>. I downloaded the model and inserted it inside my code - linking it to my assets. I Also searched for the coordinates of the fountain on google maps, <br>
![coordinates fontaine](https://user-images.githubusercontent.com/101418644/171959510-24bb323e-b84e-4121-a871-fa07cdcb36c9.JPG)
and then copy pasted them to <br>
![gps entity](https://user-images.githubusercontent.com/101418644/171959292-67d301e6-9488-4b1d-a493-6135801d2bf8.JPG) <br>
It looked like this (together with the second task) <br>
![Capture](https://user-images.githubusercontent.com/101418644/171959523-b4d34642-e3c4-4ce4-92a5-32558a5a6ed1.JPG)<br>
On the screencap above the gltf model was rotating, I edited the rotate property but later decided not to keep it since I couldn't find a way to make the text static and not follow the 3D model (as it can be seen on the picture). <br>
While uploading the code to GitHub I was suprised to discover that there's a limit of 25MB to the files, and I wasn't aware that my 3D model was _an astonishing 65MB_. So I changed it with another, simpler fountain: <br>

![stupid fountain](https://user-images.githubusercontent.com/101418644/171960155-d39979b0-a9a5-42bc-846c-c95138b1ba51.JPG) <br>

The **second task** was adding an action to the 3D model, so when clicked it shows text. I found the code for that  <a href="https://glitch.com/~salty-partner-1">here </a> . I edited it so it would fit my code. I also added _class="click"_ and _class"clickable"_ to the _a-entity_ and the _a-text_, accordingly. I copy pasted the _a-text_ from the previous deliverable, and I just changed the value of the text to the name of the fountain. It took some back and forth but I managed to get the positions and the click to work. <br>

The **third task** was editing Syros.html My place of interest was Kini Beach. I searched for the place in google maps and found it's coordinates.
![kini coordinates](https://user-images.githubusercontent.com/101418644/171952627-7a3b1201-e8e3-41ef-a6ed-118f6c6338f0.JPG)<br>
Then I found 4 images on google images of Kini and I put them inside the a-entity with the gps-entity-place. <br>
_![kini](https://user-images.githubusercontent.com/101418644/171957308-1bce63e4-a417-4174-8582-39d612c57f89.JPG)

To test if my code was working properly I added copy pasted <br>
![simulation](https://user-images.githubusercontent.com/101418644/171957572-47bcdfa5-37ae-4821-b757-1f1ace9834f0.JPG)<br>
that was given to us in the previous task 
# Conclusions
My conclusion is that from now on I will always check the size of the files that I'm using. 
Besides that, a very nice assignment. 



# Sources
<ul>
  <li> <a href="https://developer.mozilla.org/en-US/docs/Learn/Common_questions/set_up_a_local_testing_server"> Instructions on setting up a local server </a> </li>
  <li><a href="https://www.npmjs.com/package/aframe-particle-system-component"> Particle component </a> </li>
  <li> <a href="https://www.npmjs.com/package/aframe-particle-system-component"> Annyang speech command </a> </li>
  <li> <a href="https://github.com/lmalave/aframe-speech-command-component/tree/master/examples">  Public examples on github  </a></li>
  <li> <a href="https://www.color-hex.com/"> Hex codes </a> </li>
  <li> <a href="https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html"> Custom marker generator </a> </li>
  <li> <a href="https://www.youtube.com/watch?v=kVBUzAnBcck&ab_channel=NEYOVA"> Blender 3D animation turtorial </a> </li>
  <li> <a href="https://aframe.io/docs/1.3.0/components/gltf-model.html"> Gltf model A-frame </a> </li>
  <li> <a href="https://stackoverflow.com/questions/67578125/a-frame-show-gltf-model-if-variable-has-a-certain-value"> Visible atribute for a-entity </a> </li>
  <li> <a href="https://stackoverflow.com/questions/61239107/how-to-get-marker-position-x-y-ar-js"> Getting a markers position </a> </li>
  <li> <a href="https://sketchfab.com/search?type=models"> Sketchfab </a> </li>
  <li> <a href="https://sketchfab.com/3d-models/fontaine-de-lobservatoire-paris-2fd367e20a32409b9e85a812b09f152c"> Sketchfab - fontaine de l'observatoire </a> </li>
  <li> <a href="https://sketchfab.com/3d-models/medieval-fountain-empty-free-952a9c257db641229902c36abb97e8bc"> Sketchfab - Medieval fountain </a> </li>

  

  
</ul>


