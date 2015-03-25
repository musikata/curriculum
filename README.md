# musikata.curriculum
Resources related to Musikata's curriculum, including design principles and episode scripts.

## Goals

The goals of Musikata’s curriculum are:
- to help people learn to audiate
- to build musical metacognition skills
- to make audiation engaging and accessible, especially for beginners

## Inspired by Music Learning Theory

In order to effectively achieve goal (A) Musikata uses recommendations from Music Learning Theory (MLT).  MLT is a body of research that explores *how* children learn to audiate. MLT presents a framework for breaking down the process of audiation into chunks, and how to sequence those chunks. 

Note that MLT does not describe a curriculum. Instead it describes the skills that a curriculum should teach, and an effective order in which to teach those skills. 

For more information, see this [overview guide from the Gordon Institute for Music Learning](http://giml.org/docs/AboutMLT.pdf). Eric Bluestine's *[The Ways Children Learn Music](https://thewayschildrenlearnmusic.wordpress.com/)* is also a nice read, in a more conversational style.

## Structure of Musikata's Curriculum
Musikata implements its curriculum by presenting a series of episodes. Each episode does several things:
- presents music examples, to expose learners to aspects of music
- presents training exercises, to help learners build audiation skills
- presents metacognition strategies, to help learners build inner mental strength

Our challenge is to design these episodes effectively. This is not a trivial task. We must balance several competing factors, including storytelling, technological implementation, length, format, audience preferences, and many, many other factors.

It is this balancing act that makes curriculum design both challenging and interesting. It is also why we need creative and persistent people to write curriculums.

## Writing Episodes
Creating the curriculum largely consists of writing episode scriptds, and then creating media to present those scripts in an effective way.

We have come up with a format and a tool for writing effective scripts. In addition, we have guidelines and recommendations as to what makes a good episode script.

### How to Write a Script

#### Basic Guidelines
Here are guidelines and recommendations, often based on MLT:

1. KISS: Keep it simple
1. Introduce only ONE new concept at a time
1. Train ONLY rhythm or tone; do not try to do both at the same time, it can confuse beginners
1. Always introduce new concepts through musical examples first, never through pattern training. Everything must have a musical context first.

Musikata episode scripts are basically a series of commands. Like a recipe.

Scripts also describe what media resources they need (images, sounds).

In order to make it easy for a computer to understand the scripts, we write the scripts in a certain format called ‘JSON’. 

Note: a cool project for the future would be making a human-readable DSL, or a human-friendly script builder like Khan academy’s Perseus (https://github.com/Khan/perseus).

This is what a very simple script looks like:
````
{
	“assets”: [{id: “backgroundBeat”, type: “audio”, “uri”: “/media/audio/backgroundBeat.mp3”}],
“steps”: [
		[“say”, “Let’s Train”],
		[“say”, “Let’s practice rhythm today.”],
		[“audio”, {
			“id”: “backgroundBeat”,
			“action”: “start”
		}],
		[“say”, “Listen to the beat”],
		[“audio”, {
			“id”: “backgroundBeat”,
			“action”: “stop”
		}],
]
}
````

That’s the basic idea. The assets define a list of media assets to load before we start playing the script. Then the steps define a series of steps to take. In this case, we say some dialogue, and play a background beat.

Implementing a script then becomes a matter of having a script player that can handle all of the commands our script defines.
