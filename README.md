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

Other things to think about:
- spacing
- innterpolated testing, a la: <p>Szpunar K., Khan, N., Schacter, D.&nbsp;(2013):&nbsp;"<a href="https://scholar.google.com/scholar?q=Interpolated+memory+tests+reduce+mind+wandering+and+improve+learning+of+online+lectures&amp;hl=en&amp;as_sdt=0&amp;as_vis=1&amp;oi=scholart&amp;sa=X&amp;ei=SpYdVcH6HM-1ogS7zILABA&amp;ved=0CBwQgQMwAA" target="_blank">Interpolated memory tests reduce mind wandering and improve learning of online lectures</a>," <em>Proceedings of the National Academy of Sciences of the United States (PNAS).</em></p>

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

### Pacing
A well-paced curriculum allows a learner to move at a pace that matches her level. Experienced game designers know that games are most fun when they level of challenge pushes a player to the limits of his current skills. Similarly, an engaging curriculum should push a learner to advance her skills.

There are several challenges related to designing a well-paced curriculum.

#### Skill Evaluation
One challenge is how to evaluate a learner's current skill level. Skill evaluation can be difficult, for several reasons. One reason is that audiation is an opaque process. It happens inside a learner's mind, where we can not see. We can not know if she is audiating or not. We can only observe her actions.

We can gain some information from observing her actions. Can she repeate the melody we just sang? Can she name the tonality of a song?

But measuring and evaluating musical actions is also difficult. For example, if someone make a recording in his phone, it can be difficult to determine what melody he sang. Background noise and poor recording quality make it hard to deduce melodies with just software. *An interesting aside: human teachers are very good at evaluating melodies. Chalk one up for meatware.*

In addition, it can be hard to define what is musically 'correct'. What if someone sings the right notes, but it doesn't sound musical. Should that be evaluated as a 'correct' response? We wrestle with this. Music should be warm. But technology can be cold cold cold.

If you have tips or solutions on how to effectively do musical evaluation in software, we welcome your comments!

So if skill evaluation is difficult, what can we do? One possible option is to have learners self-evaluate.

#### Self-Evaluation
Self-evaluation is simple to implement. We simple ask the learner, "do you think you got it?" And she responds, "Yes", "No", or "I don't know." And we trust her.

If the learner responds "yes", we advance to the next level. If she responds "no", or "I don't know", we continue to practice at the current level.

Note that we don't want to continue practicing indefinitely. Some beginners have a tendency to obsess over getting things 'exactly right', at the expense of developing their skills more broadly. When something isn't making it sense, a better strategy is often to work on something else and then come back later. When the learner returns, the material seems fresh and new again, and she may have more insights from whatever she just learned. It's like taking a little vacation for the mind.

MLT provides us a good framework for moving around like this, because it describes ways to 'bridge' between skill levels. That is, learners don't necessarily need to proceed in sequence from one skill level to the next. They can can jump around a little.

The research of K. Szpunar et al. also suggests that self-evaluation has its own benefits. When a learner summarizes what she has learned, she integrates knowledge.

#### Peer Evaluation
Another strategy for evaluation is to use peer-evaluation. In this strategy, a student's elders would give feedback on a student's recordings, possibly on several criteria.

This approach offers several positive features:
1. It builds relationships between students.
1. It encourages the idea of teaching and progress.
1. It improves the teacher as well: when you teach something, you understand it better.
1. It scales; as more students join, they can support each other.
1. It builds a sense of community.
1. It lets humans do evaluations that would be hard for computers, for evaluating things like expressiveness, musicality, texture, etc.

It does have some risks:
1. Making sure that the quality of peer feedback is high and not negative.
1. Supply/demand balance. Will there be enough advanced students to help beginning students?

There may be some ways to incentivize teaching and coaching too. Game points, social badges, rewards, reputation, or gifts.


#### Content Matching
If we assume that we can determine a learner's skill level (through self-evaluation or other means), then our next challenge is to provide material at the right level of challenge.

Digital media offer us some interesting ways to approach this challenge, in ways that are not always possible in other media. We can design 'atoms' or 'molecules' of content, where each molecule is associated with a skill level. We can then dynamically tailor episodes for learners by combining molecules with the appropriate skill levels. 

For example, a learner may be at the level of sub-dominant aural recognition in tonal learning sequence, but only at macro/micro beat aural recognition in rhythmic learning sequence. We could assemble an episode on-the-fly that combines (1) a rote song with macro/micro beats and (2) sub-dominant tonal patterns.

However, dynamic episode assembly can also be challenging. How do we create the molecules of learning? How do we weave them together so that episodes still feel cohesive? How do we tie-in story elements, if we don't know the specific structure of each episode?

Contrast dynamic episode creation with static episode creation, as used in the JRI series. The JRI describes a set of static episodes. However, music teachers often reassemble the static episodes depending on the levels of their students. So in many ways, music teachers already do dynamic episode creation. Just not in algorithmic way.


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
