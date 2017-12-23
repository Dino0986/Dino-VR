# <center > **Sketchup To JanusVR (With Blender)** </center> 
 	Ver 0.1 CC Dave K
 
---
#### Intro: 
#####  Making models in Sketchup is easy, making good models isn't. When exporting from Sketchup, lots of people don't have properly flipped normals, or watertight meshes. Sketchup does a very poor job of explaining this to the users and when the models stay in Sketchup is generally fine, problems occur when exporting to other programs that want cleaner models. I hope this guide can be useful for someone hoping to get their model from Sketchup to VR.

---

#### -  Step 0 : Prerequisites. Things to install before you start.

1. Sketchup: I use the pro version, it allows for more kinds of file export and the use of solid tools. Any version after 2014 is fine for this. The free version (Sketchup Make) is fine, but I would not recommend it. Cracked versions can be found online fairly easily.
   
   - Sketchup Plugins:
       1. [TT LIB^2](https://extensions.sketchup.com/content/tt_lib%C2%B2): A library used by a lot of plugins from [ThomThom](https://extensions.sketchup.com/user/261)
       1. [Solid Inspector 1](https://extensions.sketchup.com/en/content/solid-inspector): This is the first version of solid inspector, it outlines the sections of your model that are broken. Is harder to use than Solid Inspector^2, but has more features.
       1. [Solid Inspector^2](https://extensions.sketchup.com/en/content/solid-inspector%C2%B2): Does most of the same things as the first version, but with a nicer interface that is better for checking your model as you build it. Anything this version doesn't catch, version 1 will.
       1. [Shape Bender](https://extensions.sketchup.com/en/content/clf-shape-bender): More of a quality of life tool. Nice to have for modelling, but not needed.
       1. [ LibFreedo6](https://extensions.sketchup.com/en/content/libfredo6-0): Needed for round corner, another library for some useful plugins.
       1.  [Round Corner](https://extensions.sketchup.com/en/content/roundcorner): Another quality of life tool, lets you chamfer and fillet corners easily. Nice if you want to make anything with rounded corners. Not required, but is nice to have and I will be using it during this tutorial.
			
	#####	//Sidenote: you can use any other plugins you want, these are just my favourite and I use them a lot, and will be using them heavily in this guide.

1. Blender: It's free, free as in freedom. Grab it from [here](https://www.blender.org/), this tutorial will use 2.78. Any version should work. As long as it has the cycles renderer.
1. JanusVR, any version will do. Steam or standalone builds, most of this will also work in [JanusWeb](https://web.janusvr.com/).

---

#### -  Step 1 : Setting Up Sketchup  


- Open sketchup and pick any template, remove endpoints and extensions if enabled by the template by default, leave profiles and edges enabled. I use feet and inches for architecture.  
 
##### This window is opened from the 'Windows' tab and by selecting 'Styles'

![alt text](https://raw.githubusercontent.com/Dino0986/Dino-VR/gh-pages/Sketchup-Janus/styles.png "Styles") ![alt text](https://raw.githubusercontent.com/Dino0986/Dino-VR/gh-pages/Sketchup-Janus/styles2.png "Styles Without Endpoints and Extension")


- Delete Sophie, or keep her if you want a human sized object. I find it easier to just remove her now, scale everything to itself and then make things human sized afterwords. This is why I use the feet and inches template. 

##### I can visualise how big things are in real life in feet and inches. If you use metric, go ahead and just visualize things in MM.

 ![alt text](https://raw.githubusercontent.com/Dino0986/Dino-VR/gh-pages/Sketchup-Janus/sophie.png "Styles")

---

#### -  Step 2 : Picking a style and getting started
1. Start modelling! Start small, making large models requires lots of work, and is a great way to burn yourself out before you make anything you are proud of. Think of a simple scene. Something like a park bench, campfire, bedroom, or street corner are great starting points. Try to pick something within your skill set, don't over reach and make sure you feel comfortable with the way Sketchup works.
1. Pick a style and stick with it, if you change styles while your final product will look very unity store esque. I use a very low poly stylized style. 
2. You can texture with Sketchup, but its texturing tools are very limited, while also producing very poor UV maps. These UV's can be used, as .dae files can have multiple UV maps, and Janus supports this. UV maps are used to tell the software where your textures should be on the model, blender can auto generate UV's for you, but these should not be used if you intend on having hand painted textures.

##### This a screenshot from JanusVR, after baking shadows using blender. This Beetle has no textures other than shadows, the rest are vertex colours.
	
![alt text](https://raw.githubusercontent.com/Dino0986/Dino-VR/gh-pages/Sketchup-Janus/beetle.png "Beetle")

---

#### -  Step 2 : Actually starting to model.

- I'm going to make a little street corner with a couple tables, chairs, and a faux storefront for an imaginary coffee shop. From here on out, most of this guide will be silent videos with a text write up to go along with.

##### **All keyboard shorcuts are in the bottom left corner, as well as being in brackets in the write up. **

1. 0:00 Starting with a square(R), I used a 10'x10' square(R) and extruded(P) it up 3".
2. 0:20 Then I offset(F) the rear 2 edges 5' towards the middle of the square.
3. 0:30 Then I extruded(P) the L shaped section up 3".
4. 0:38 Using the offset(F) tool again I offset the inside edges 4" to make the curb.
5. 0:42 Then I extruded(P) the curb a half inch above the L shape.
6. Then, using round corner, I added a fillet to the curb. Round corner works by first selecting the edges you want to modify and then clicking on either fillet or chamfer. After you select what style you want you type a number, this number is how long the modification will be, measured from the corner in. I used 1".
7. 1:00 As a final step, I used the eraser(E) and the shift key modifier to un-soften the edges. This allows you to see your edges so you can select them later. A good practice for anyone using roundcorner.

<iframe width="740" height="400" src="https://www.youtube.com/embed/DJFW-Lft-cQ" frameborder="0" gesture="media" allow="encrypted-media" allowfullscreen></iframe>
