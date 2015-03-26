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

## General Structure of Musikata's Curriculum: Episodes
Musikata implements its curriculum by presenting a series of episodes. Each episode does several things:
- presents music examples, to expose learners to aspects of music
- presents training exercises, to help learners build audiation skills
- presents metacognition strategies, to help learners build inner mental strength

Each episode should be designed with to achieve immediate short-term goals ("sequential objectives" in MLT terminology), and to bring the learner closer towards longer-term goals ("comprehensive objectives").

Our challenge is to design these episodes effectively. This is not a trivial task. We must balance several competing factors, including storytelling, technological implementation, length, format, audience preferences, and many, many other factors.

It is this balancing act that makes curriculum design both challenging and interesting. It is also why we need creative and persistent people to write curriculums.

## Learning from Existing Curricula
We have much to learn from existing curriculum implementations.

If you are interested in curriculum design, it is well worth studying the "Jump Right In" (JRI) series of instructional books. The JRI books present MLT-inspired curriculums that have been put into use and have been tested in real classrooms. Much thought has gone into the JRI series, and several MLT researchers have contributed to the series. 

I (Alex) especially recommend the Teachers's Guide for Recorder.

The JRI series is intended primarily for in-classroom teaching. It is worth thinking about how we can adapt JRI sequencing and lessons to online formats.

For example, the JRI recorder curriculum is designed for classes that meet twice per week. Each week corresponds to one unit in the JRI book, and each unit has two sections. The JRI curriculum provides audiation exercises and executive exercises (not excel spreadsheets, but physically controlling an instrument ;) ) to practice between lessons.

It is not clear yet how (or if) we adapt this approach to an online curriculum. Does it make sense to have different types of episodes? For example, we may choose to have 'big' episodes that correspond to JRI teaching sessions, with 'little' practice episodes in-between, corresponding to what a student would practice outside of class.

Or it may make sense to have one type of episode, and we sprinkle in new content and practice review throughout. These things are not clear yet.

The JRI presents a typical lesson structure which may be useful. Each JRI lesson is structured like this:

1.
 a. Learning a rote song.
 b. Building coordination for rhythmic motion
 c. Administrative stuff
 d. building coordination for instrumental control
 e. practice tips
2. 
 a. Rhythm or Tone Patterns
 b. Melodic patterns
3. Suggestions for practicing with the Home-Study CD

This structure is common to all the lesson units in the JRI recorder curriculum. It is designed for the episode format of JRI lessons (2 lessons per week), and the media (in-class presentation, CD recording for home use).

It is not clear yet whether this structure is a good fit for Musikata's episode format. Musikata can provide episodes at any time, on any schedule. Musikata uses different media (web pages). So it's not clear yet whether we should follow the same structure. It is likely that we will want to change somethings, especially due to differences in media and episode scheduling.

## Sequencing
MLT provides a framework for thinking about sequencing, but only a framework. There is still a great deal of flexibility in how musical content should be presented. In this section we discuss a few general ideas.

### Beginning Preparation
It is important to prepare beginners appropriately for more advanced concepts. The JRI Recorder Teacher's Guide offers several tips:
1. Build musical vocabulary with rote songs first before training with patterns. It is important that learners have musical examples in their minds, to give context to patterns.
1. Make sure that the feeling of flowing rhythmic motion is established. The JRI Recorder book provides several useful exercises for doing this.

## Writing Episodes
Creating the curriculum largely consists of writing episode scripts, and then creating media to present those scripts in an effective way.

We need to come up with a format and a tool for writing effective scripts. In addition, we have guidelines and recommendations as to what makes a good episode script.

Then we need to make a tool to present those scripts. You can find some thoughts about presentation in this repo: https://github.com/musikata/musikata.kabuki.

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
