## Machine Learning Examples
### 1. Problem Solving and Search
- How can we find the shortest distance between point a --> point b
### 2. Game playing
- Computers can play games by traversing searching a tree using a special type of search
	- Adversarial Search
### 3. Classification Examples
- Ability to predict if a new patient is at high-risk for emergency C-section from historical patient records based off 215 attributes
### 4. Clustering Example
- Ability to group countries based on their similarity in quality of life factors
	- Example of unsupervised learning

## What is AI?
- Think like humans?
- Act like humans?
- Think rationally?
- Act rationally?
What is rationality?
- Ideal performance given a performance measure
What is to act rationally?
- Selecting the best action at each step
- The one that maximizes the given performance measure

### 1. Acting Humanly - Turing Test Approach
- Proposed by Alan Turing in 1950
- Asked the question, "Can machines think? If so, how could we tell?"
- "Thinking" is difficult to define and Alan Turing created a **test**
	- This test has a human interrogator asks written questions and receives back written responses
	- A computer passes the test if the human interrogator cannot tell if the response came from a human or a computer
#### What would a computer need to pass the Turing Test?
- **Natural language processing** - Communicate successfully in written English
- **Knowledge representation** - Store what is knows and hear (memory)
- **Automated reasoning** - Used stored information to answer questions and draw conclusions
- **Machine learning** - Adapt to new situations and detect patterns and apply to new situations
#### The Total Turing Test
In the total Turing test, in addition to written English, an interrogator should be able to test the subject's perceptual abilities. Then, the computer would need:
- **Computer vision** to perceive objects
- **Robotics** to move them around

#### The Turing Test isn't that important
Within the AI community, there is little effort into trying to pass the Turing test because **a machine that resembles a human being isn't very useful**.

- We can explain with an analogy:
When the Wright brothers succeeded building an airplane, did they:
- Try to imitate how birds fly?
- Learned basic aerodynamics?
Clearly, in this example it is when they learned aerodynamics and the same principles is used for AI

#### The Reverse Turing Test - CAPTCHA
- CAPTCHA stands for "Completed Automated Public Turing test to tell Computers and Humans Apart"
- proposed by Luis Von Ahn and Manuel Blum from CMU
- Called the "reverse" Turing test because it is trying to see if it is a human not a robot

### 2. Thinking Humanly: Cognitive Modelling Approach
Before we try to program a computer to think, we should ask how do humans think?
- Given a problem, it is not enough that it is solved correctly by a computer but also with the same reasoning as a human should follow
To answer the question "how do humans think?"
- Cognitive Science: Constructs and tests theories of how the human mind works using methods from psychology and computer models
	- Note that Cognitive Science and AI are separate fields
The first program to embody the "humane thinking" is the General problem Solver (GPS)
- Program for proving theorems and solving geometric problems
- Imitates human reasoning:
	- The way it consider goals and sub-goals is similar to humans

### 3. Thinking Rationally: The "Laws of Thought" Approach
In this approach, our goal is to build intelligent systems
- Take a description of a problem in logical notation
- Finds the solution using correct inference
	- From "Socrates is a man, All man are mortal"
	- It can infer that "Socrates is mortal"
- Problems:
	- Ability to take informal knowledge and represent it  in formal notation
		- Especially difficult when knowledge is uncertain
	- Limited time and memory

### 4. Acting Rationally: The Rational Agent Approach
An intelligent Agent should have these properties:
- Built-in knowledge and goals
- Perceives the environment
- Acts rationally to achieve its goals using its knowledge 
- Acts rationally - Does the right thing
	- Performs the action that maximizes a performance measure
In real-life scenarios, it is much more complex and as a result:
- Always doing the right thing is not possible
	- Too much computational demands
	- Limited rationality - acts appropriately when there is not enough time to make all computations

## Foundations of AI
Artificial Intelligence is founded by many different disciplines, this includes:
- Philosophy
- Mathematics
- Psychology
- Linguistics
- Computer Engineering

## Gestation (1943-1955)
McCulloch and Pitt's created a mathematical model of an artificial neuron in 1943
- A neuron is either "on" or "off"
	- "On" where there is sufficient stimulation from neighbouring neurons
	- "Off" when there is NOT sufficient stimulation from neighbouring neurons
- This artificial neuron mathematically weighted sum of input signals and is compared to a threshold to either output 1 or 0
![[Pasted image 20240219221156.png]]
In 1950, Hebb proposed a rule for modifying the connection strength between neurons
- This rule is coined as Hebbian learning and is still used in neural networks

In 1950, Alan Turing also proposed the idea of teaching a computer its intelligence instead of programming by hand
- This idea was revolutionary at the time

In 1951, Minsky and Edmonds built the first neural network computer
- Network of 40 neurons using 3000 vacuum tubes

### Birth (1956)
In 1956, John McCarthy's organized a 2-month workshop for researchers interested in automata theory, neural networks, and the study of intelligence
- In this workshop, it is where the birth of AI was done

### Early Enthusiasm (50-60s)
In 1960s, researchers have created a program called a Perceptrons which has the ability to learn from examples
- The first perceptron was used to differentiate males and females
In the 1959 - 1975, Programs for playing checkers were made which developed:
- Alpha-beta pruning - Pruning unnecessary branches of the game tree
- Disproved the idea that computers can do only what they are told to do
	- Programs were able to learn from experience
#### High Expectation
The great progress in AI in the 50-60s gave researchers an unrealistic high expectations 

### A Dose of Reality (60-70s)
In the 60-70s the development of AI slowed down and researchers got a dose of reality
- Problem 1: Limitations of algorithms
	- 1960 - Minsky and Papert demonstrated the limitations of existing neural networks
		- A need for more complex networks and a new learning rule
- Problem 2: Need for deeper knowledge 
	- Syntactic manipulation is not sufficient
		- e.g. Translation Russian -> English
		- "The spirit is willing but the flesh is weak" -> "The vodka is good but the meat is rotten"
- Problem 3: Many real problems are intractable
	- When trying to generalize to larger problems, it proved to be more difficult
		- Needs to deal with combinatorial explosion + Computing power wasn't sufficient

### Come Back (From the 70s)
- In the 70s, Knowledge-based systems became really popular as they were able to solve specific problems in restricted domains. 
- It was able to provide expert quality advice, diagnosed and recommend for real-world problems
![[Pasted image 20240219224708.png]]
- In the 80s, neural networks returned to popularity as Rumelhart and McClelland created a backpropagation algorithm for training multilayer

### Today - Machine Learning 
Today, machine learning and data mining are the fastest growing areas in AI
- Big Data, Deep Learning
The reason why deep learning has gotten a lot of attention was because we now have super powerful computers capable of performing deep learning

### Rise of Machine Learning
- Lots of data is being collected
	- Trillions of words in English, Images on the web, genomic sequences
	- Weather data, supermarket transactions, government statistics, medical records, user data, movies watched, etc.
- This data can be used to:
	- Extract useful patterns for different types of analytics
	- Train machines to learn to perform different tasks
		- Translate languages
		- Drive vehicles
		- 