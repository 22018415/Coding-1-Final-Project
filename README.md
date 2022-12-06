# Coding-1 Final Project by Yufei Ma
Hello! Welcome to my final project of coding one. My project is a based on GLSL and JavaScript. It is called "Chaos".   
You can see it on mimic: https://mimicproject.com/code/01217a80-1c8c-0b13-8b75-e593341fbcee

## Contents
* [Introduction](#40)
* [Highlights](#41)
* [Difficulties I Met](#42)


<h2 id="40">Introductinon</h3>
For almost a year, I was in a chronic state of dislocation and emotion. Talking to myself, confronting and arguing with myself.  

I visualised and audio-visualised the intentions I felt in my chaotic thoughts, trying to find some order in my confused thoughts.  
This paradox allows order and random chaos to coexist.    
  
I was inspired by a dream I had during a chaotic period, which was filled with colourful splotches and mosaics, like patches of light that would appear in front of me when I closed my eyes to the sun. And I was trying to make sounds and connect with the outside world in these chaotic colours. At first, it was a shrill cry for help, then it turned into a repetitive drowsy murmur, as if whispering some weekly verse. Interspersed from time to time are the sounds of some kind of musical instrument. This dream seemed to me to have been seen many times before, it was so familiar and unreal.

<h2 id="41">Highlights</h3>
<h3>Shader calculation based on the example on mimic  </h3>

    vec3 p = vec3((gl_FragCoord.xy+resolution/3.0)/(resolution.y),mouse.x);

			for (int i = 0; i < 21; i++)
    		{
	   			p = abs((abs(p)/dot(p, p)-0.4));
	   			if(length(p) > 1.0 && length(p) < 1.01)break;
			}
            
			gl_FragColor.rgb = p;

<h2 id="42">Difficulties I met</h3>
When I tried to learn the shader in more depth, I encountered a number of difficulties. Firstly, it was coded in GLSL, a C-like language, which I had never come across before. Therefore, it took me a lot of time to learn the basics of C++ before I could start to understand the logic of how GLSL works.  

I then experimented with many different ways of sampling and outputting the music. At first, it was all very difficult for me to move away from the original form of music, and I made music that was based on the original melodic base, unable to create my own melodies. After studying other students' excellent assignments, I modified and experimented with the code over and over again and eventually modified it to produce an okay melody. (In a sense, chaos is also my theme)

