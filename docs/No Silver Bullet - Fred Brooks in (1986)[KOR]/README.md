# 은탄환은 없다 - 소프트웨어 공학의 본질과 우연성

Frederick P. Brooks, Jr.  
University of North Carolina at Chapel Hill

> There is no single development, in either technology or management technique,
which by itself promises even one order-of-magnitude improvement within a decade in productivity,
in reliability, in simplicity.

## Abstract<sup>1</sup>
All software construction involves essential tasks,
the fashioning of the complex conceptual structures that composethe abstract software entity,
and accidental tasks, the representation of these abstract entities in programming languages
and the mapping of these onto machine languages within space and speed constraints.
Most of the big past gains in software productivity have come from removing artificial
barriers that have made the accidental tasks inordinately hard,
such as severe hardware constraints, awkward programming languages,
lack of machine time. How much of what software engineers now do is
still devoted to the accidental, as opposed to the essential?
Unless it is more than 9/10 of all effort, shrinking all the accidental activities
to zero time will not give an order of magnitude improvement.  
 &nbsp;
 Therefore it appears that the time has come to address
the essential parts of the software task,
those concerned with fashioning abstract conceptual structures of great complexity.
I suggest:
- Exploiting the mass market to avoid constructing what can be bought.
- Using rapid prototyping as part of a planned iteration in establishing software requirements. 
- Growing software organically, adding more and more function to systems as they are run, used, and tested. 
- Identifying and developing the great conceptual designers of the rising generation. 

## Introduction
&nbsp; Of all the monsters who fill the nightmares of our folklore,
none terrify more than werewolves, because they transform unexpectedly
from the familiar into horrors. For these, we seek bullets of silver
than can magically lay them to rest.  
 &nbsp;
 The familiar software project has something of this character
(at least as seen by the non-technical manager),
usually innocent and straightforward,
but capable of becoming a monster of missed schedules, blown budgets,
and flawed products. So we hear desperate cries for a silver bullet,
something to make software costs drop as rapidly as computer hardware costs do.  
 &nbsp;
 But, as we look to the horizon of a decade hence,
we see no silver bullet. There is no single development,
in either technology or management technique,
which by itself promises even one order of magnitude improvement in productivity,
in reliability, in simplicity. In this chapter we shall try to see why,
but examining both the nature of the software problem and the properties of
the bullets proposed.  
 &nbsp;
 Skepticism is not pessimism, however.
Although we see no startling breakthroughs,
and indeed, believe such to be inconsistent with the nature of software,
many encouraging innovations are under way.
A disciplined, consistent effort to develop, propagate,
and exploit them should indeed yield an order-of-magnitude improvement.
There is no royal road, but there is a road.  
 &nbsp;
 The first step toward the management of disease was replacement of
demon theories and humours theories by the germ theory.
That very step, the beginning of hope, in itself dashed all hopes of magical solutions.
It told workers the progress would be made stepwise, at great effort,
and that a persistent, unremitting care would have to be paid to a discipline of
cleanliness. So it is with software engineering today.  
 &nbsp;

## Does It Have To Be Hard? – Essential Difficulties
Not only are there no silver bullets now in view, the very nature of software makes it unlikely that there will be any−no inventions that will do for software productivity, reliability, and simplicity what electronics, transistors, and large-scale integration did for computer hardware. We cannot expect ever to see twofold gains every two years.  
&nbsp;
First, we must observe that the anomaly is not that software progress is so slow but that computer hardware progress is so fast. No other technology since civilization began has seen six orders of magnitude price-performance gain in 30 years. In no other technology can one choose to take the gain in either improved performance or in reduced costs. These gains flow from the transformation of computer manufacture from an assembly industry into a process industry.  
&nbsp;
Second, to see what rate of progress we can expect in software technology, let us examine its difficulties. Following Aristotle, I divide them into essence−the difficulties inherent in the nature of the software−and accidents−those difficulties that today attend its production but that are not inherent.  
&nbsp;
The accidents I discuss in the next section. First let us consider the essence.  
&nbsp;
The essence of a software entity is a construct of interlocking concepts: data sets, relationships among data items, algorithms, and invocations of functions. This essence is abstract, in that the conceptual construct is the same under many different representations. It is nonetheless highly precise and richly detailed.  
&nbsp;
I believe the hard part of building software to be the specification, design, and testing of this conceptual construct, not the labor of representing it and testing the fidelity of the representation. We still make syntax errors, to be sure; but they are fuzz compared to the conceptual errors in most systems.  
&nbsp;
If this is true, building software will always be hard. There is inherently no silver bullet.  
&nbsp;
Let us consider the inherent properties of this irreducible essence of modern software systems: complexity, conformity, changeability, and invisibility.  

**Complexity.** Software entities are more complex for their size than perhaps any other human construct, because no two parts are alike (at least above the statement level). If they are, we make the two similar parts into one, a subroutine, open or closed. In this respect software systems differ profoundly from computers, buildings, or automobiles, where repeated elements abound.  
&nbsp;
Digital computers are themselves more complex than most things people build; they have very large numbers of states. This makes conceiving, describing, and testing them hard. Software systems have orders of magnitude more states than computers do.  
&nbsp;
Likewise, a scaling-up of a software entity is not merely a repetition of the same elements in larger size; it is necessarily an increase in the number of different elements. In most cases, the elements interact with each other in some nonlinear fashion, and the complexity of the whole increases much more than linearly.  
&nbsp;
The complexity of software is in essential property, not an accidental one. Hence descriptions of a software entity that abstract away its complexity often abstract away its essence. Mathematics and the physical sciences made great strides for three centuries by constructing simplified models of complex phenomena, deriving properties from the models, and verifying those properties experimentally. This worked because the complexities ignored in the models were not the essential properties of the phenomena. It does not work when the complexities are the essence.  
&nbsp;
Many of the classical problems of developing software products derived from this essential complexity and its nonlinear increased with size. From the complexity comes the difficulty of communication among team members, which leads to product flaws, cost overruns, schedule delays. From the complexity comes the difficulty of enumerating, much less understanding, all the possible states of the program, and from that comes the unreliability. From the complexity of the functions comes the difficulty of invoking those functions, which makes programs hard to use. From complexity of structure comes the difficulty of extending programs to new functions without creating side effects. From the complexity of structure comes the unvisualized state that that constitute security trapdoors.  
&nbsp;
Not only technical problems but management problems as well come from the complexity. This complexity makes overview hard, thus impeding conceptual integrity. It makes it hard to find and control all the loose ends. It creates the tremendous learning and understanding burden that makes personnel turnover a disaster.

**Conformity.** Software people are not alone in facing complexity. Physics deals with terribly complex objects even at the “fundamental” particle level. The physicist labors on, however, in a firm faith that there are unifying principles to be found, whether in quarks or in unified field theories. Einstein repeatedly argued that there must be simplified explanations of nature, because God is not capricious or arbitrary.  
&nbsp;
No such faith comforts the software engineer. Much of the complexity he must master is arbitrary complexity, forced without rhyme or reason by the many human institutions and systems to which his interfaces must confirm. These differ from interface to interface, and from time to time, not because of necessity but only because they were designed by different people, rather than by God.  
&nbsp;
In many cases the software must confirm because it has most recently come to the scene. In others it must conform because it is perceived as the most conformable. But in all cases, much complexity comes from conformation to other interfaces; this cannot be simplified out by any redesign of the software alone.

**Changeability.** The software entity is constantly subject to pressures for change. Of course, so are buildings, cars, and computers. But manufactured things are infrequently changed after manufacture; they are superseded by later models, or essential changes are incorporated in later serial-number copies of the same basic design. Callbacks of automobiles are really quite infrequent; field changes of computers somewhat less so. Both are much less frequent than modifications to fielded software.  
&nbsp;
Partly this is because the software in a system embodies its function, and the function is the part that most feels the pressures of change. Partly it is because software can be changed more easily−it is pure thought-stuff, infinitely malleable. Buildings do in fact get changed, but the high costs of change, understood by all, serve to dampen the whim of the changers.  
&nbsp;
All successful software gets changed. Two processes are at work. As a software product is found to be useful, people try it in new cases at the edge of, or beyond, the original domain. The pressures for extended function come chiefly from users who like the basic function and invent new uses for it.  
&nbsp;
Second, successful software also survives beyond the normal life of the machine vehicle for which it is first written. If not new computers, then at least new disks, new displays, new printers come along; and the software must be conformed to its new vehicles of opportunity.  
&nbsp;
In short, the software product is embedded in a cultural matrix of applications, users, laws, and machine vehicles. These all change continually, and their changes inexorably force change upon the software product.

**Invisibility.** Software is invisible and unvisualizable. Geometric abstractions are powerful tools. The floor plan of a building helps both architect and client evaluate spaces, traffic flows, and views. Contradictions become obvious, omissions can be caught. Scale drawings of mechanical parts and stick-figure models of molecules, although abstractions, serve the same purpose. A geometric reality is captured in a geometric abstraction.  
&nbsp;
The reality of software is not inherently embedded in space. Hence it has no ready geometric representation in the way that land has maps, silicon chips have diagrams, computers have connectivity schematics. As soon as we attempt to diagram software structure, we find it to constitute not one, but several, general directed graphs, superimposed one upon another. The several graphs may represent the flow of control, the flow of data, patterns of dependency, time sequence, name-space relationships. These are usually not even planar, much less hierarchical. Indeed, one of the ways of establishing conceptual control over such structure is to enforce link cutting until one or more of the graphs becomes hierarchical.<sup>2</sup>  
&nbsp;
In spite of progress in restricting and simplifying the structures of software, they remain inherently unvisualizable, thus depriving the mind of some of its most powerful conceptual tools. This lack not only impedes the process of design within one mind, it severely hinders communication among minds.

## Past Breakthroughs Solved Accidental Difficulties
If we examine the three steps in software technology that have been most fruitful in the past, we discover that each attacked a different major difficulty in building software, but they have been the accidental, not the essential, difficulties. We can also see the natural limits to the extrapolation of each such attack.

**High-level languages.** Surely the most powerful stroke for software productivity, reliability, and simplicity has been the progressive use of high-level languages for programming. Most observers credit that development with at least a factor of five in productivity, and with concomitant gains in reliability, simplicity, and comprehensibility  
&nbsp;
What does a high-level language accomplish? It frees a program from much of its accidental complexity. An abstract program consists of conceptual constructs: operations, data types, sequences, and communication. The concrete machine program is concerned with bits, registers, conditions, branches, channels, disks, and such. To the extent that the high-level language embodies the constructs wanted in the abstract program and avoids all lower ones, it eliminates a whole level of complexity that was never inherent in the program at all.  
&nbsp;
The most a high-level language can do is to furnish all the constructs the programmer imagines in the abstract program. To be sure, the level of our sophistication in thinking about data structures, data types, and operations is steadily rising, but at an ever-decreasing rate. And language development approaches closer and closer to the sophistication of users.  
&nbsp;
Moreover, at some point the elaboration of a high-level language becomes a burden that increases, not reduces, the intellectual task of the user who rarely uses the esoteric constructs.

**Time-sharing.** Most observers credit time-sharing with a major improvement in the productivity of programmers and in the quality of their product, although not so large as that brought by high-level languages.  
&nbsp;
Time-sharing attacks a distinctly different difficulty. Time-sharing preserves immediacy, and hence enables us to maintain an overview of complexity. The slow turnaround of batch programming means that we inevitably forget the minutiae, if not the very thrust, of what we were thinking when we stopped programming and called for compilation and execution. This interruption of consciousness is costly in time, for we must refresh. The most serious effect may well be the decay of grasp of all that is going on in a complex system.  
&nbsp;
Slow turn-around, like machine-language complexities, is an accidental rather than an essential difficulty of the software process. The limits of the contribution of time-sharing derive directly. The principle effect is to shorten system response time. As it goes to zero, at some point it passes the human threshold of noticeability, about 100 milliseconds. Beyond that no benefits are to be expected.

**Unified programming environments.** Unix and Interlisp, the first integrated programming environments to come into widespread use, are perceived to have improved productivity by integral factors. Why?  
&nbsp;
They attack the accidental difficulties of using programs together, by providing integrated libraries, unified file formats, and piles and filters. As a result, conceptual structures that in principle could always call, feed, and use one another can indeed easily do so in practice.  
&nbsp;
This breakthrough in turn stimulated the development of whole toolbenches, since each new tool could be applied to any programs by using the standard formats.  
&nbsp;
Because of these successes, environments are the subject of much of today’s software engineering research. We will look at their promise and limitations in the next section.

## Hopes for the Silver
Now lets us consider the technical developments that are most often advanced as potential silver bullets. What problems do they address? Are they the problems of essence, or are they remainders of our accidental difficulties? Do they offer revolutionary advances, or incremental ones?

**Ada and other high-level language advances.** One of the most touted recent developments is the programming language Ada, a general-purpose, high-level language of the 1980s. Ada indeed not only reflects evolutionary improvements in language concepts but embodies features to encourage modern design and modularization concepts. Perhaps the Ada philosophy is more of an advance than the Ada language, for it is the philosophy of modularization, of abstract data types, of hierarchical structuring. Ada is perhaps over-rich, the natural product of the process by which requirements were laid on its design. That is not fatal, for subset working vocabularies can solve the learning problem, and hardware advances will give us the cheap MIPS to pay for the compiling costs. Advancing the structuring of software systems is indeed a very good use for the increased MIPS our dollars will buy. Operating systems, loudly decried in the 1960s for their memory and cycle costs, have proved to be an excellent form in which to use some of the MIPS and cheap memory bytes of the past hardware surge.  
&nbsp;
Nevertheless, Ada will not prove to be the silver bullet that slays the software productivity monster. It is, after all, just another high-level language, and the biggest payoff from such languages came from the first transition, up from the accidental complexities of the machine into the more abstract statement of step-by-step solutions. Once those accidents have been removed, the remaining ones are smaller, and the payoff from their removal will surely be less.  
&nbsp;
I predict that a decade from now, when the effectiveness of Ada is assessed, it will be seen to have made a substantial difference, but not because of any particular language feature, nor indeed because of all of them combined. Neither will the new Ada environment prove to be the cause of the improvements. Ada’s greatest contribution will be that switching to it occasioned training programmers in modern software design techniques.

**Object-oriented programming.** Many students of the art hold out more hope for object-oriented programming than for any of the other technical fads of the day.<sup>3</sup> I am among them. Mark Sherman of Dartmouth notes that we must be careful to distinguish two separate ideas that go under that name: abstract data types and hierarchical types, also called classes. The concept of the abstract data type is that an object’s type should be defined by a name, a set of proper values, and a set of proper operations, rather than its storage structure, which should be hidden. Examples are Ada packages (with private types) or Modula’s modules.  
&nbsp;
Hierarchical types, such as Simula-67’s classes, allow the definition of general interfaces that can be further refined by providing subordinate types. The two concepts are orthogonal−there may be hierarchies without hiding and hiding without hierarchies. Both concepts represent real advances in the art of building software.  
&nbsp;
Each removes one more accidental difficulty from the process, allowing the designer to express the essence of his design without having to express large amounts of syntactic material that add no new information content. For both abstract types and hierarchical types, the result is to remove a higher-order sort of accidental difficulty and allow a higher-order expression of design.  
&nbsp;
Nevertheless, such advances can do no more than to remove all the accidental difficulties from the expression of the design. The complexity of the design itself is essential; and such attacks make no change whatever in that. An order-of-magnitude gain can be made by object-oriented programming only if the unnecessary underbrush of type specification remaining today in our programming language is itself responsible for nine-tenths of the work involved in designing a program product. I doubt it.

**Artificial intelligence.** Many people expect advances in artificial intelligence to provide the revolutionary breakthrough that will give order-of-magnitude gains in software productivity and quality.<sup>4</sup> I do not. To see why, we must dissect what is meant by “artificial intelligence” and then see how it applies.
>**Parnas has clarified the terminological chaos:**<br><br>
*Two quite different definitions of AI are in common use today. AI-1: The use of computers to solve problems that previously could only be solved by applying human intelligence. AI-2: The use of a specific set of programming techniques knows as heuristic or rule-based programming. In this approach human experts are studies to determine what heuristics or rules of thumb they use in solving problems... The program is designed to solve a problem the way that humans seem to solve it.
The first definition has a sliding meaning... Something can fit the definition of AI-1 today but, once we see how the program works and understand the problem, we will not think of it as AI anymore... Unfortunately I cannot identify a body of technology that is unique to this field... Most of the work is problem-specific, and some abstraction or creativity is require to see how to transfer it.<sup>5</sup>*

I agree completely with this critique. The techniques used for speech recognition seem to have little in common with those used for image recognition, and both are different from those used in expert systems. I have a hard time seeing how image recognition, for example, will make any appreciable difference in programming practice. The same is try of speech recognition. The hard thing about building software is deciding what to say, not saying it. No facilitation of expression can give more than marginal gains.  
&nbsp;
Expert systems technology, AI-2, deserves a section of its own.

