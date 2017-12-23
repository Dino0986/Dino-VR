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

#### -  Step 2 : Making a Decent Sketchup Model  

Start modelling! 