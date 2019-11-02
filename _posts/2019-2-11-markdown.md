---
layout: post
title: markdown & pandoc
---

## 19.


Modeling: A Study in Words and Meanings
=======================================

Willard McCarty
---------------

> Out on site, you were never parted from your plans. They were your
> Bible. They got dog-eared, yellowed, smeared with mud, peppered with
> little holes from where you had unrolled them on the ground. But
> although so sacred, the plans were only the start. Once you got out
> there on the site everything was different. No matter how carefully
> done, the plans could not foresee the variables. It was always
> interesting, this moment when you saw for the first time the actual
> site rather than the idealised drawings of it. He knew men who hated
> the variables. They had their plans and by golly they were going to
> stick to them. If the site did not match the drawings it was like a
> personal insult. He himself liked the variables best. He liked the way
> that the solution to one problem created another problem further down
> the line, so that you had to think up something else, and that in turn
> created another problem to solve. It was an exchange, backwards and
> forwards. Some men thought of it as a war, but to him it was more like
> a conversation. Kate Grenville, The Idea of Perfection (Sydney:
> Picador, 1999): 62--3

Introduction
============

The question of modeling arises naturally for humanities computing from
the prior question of what its practitioners across the disciplines have
in common. What are they all doing with their computers that we might
find in their diverse activities indications of a coherent or cohesible
practice? How do we make the best, most productive sense of what we
observe? There are, of course, many answers: practice varies from person
to person, from project to project, and ways of construing it perhaps
vary even more. In this chapter I argue for modeling as a model of such
a practice. I have three confluent goals: to identify humanities
computing with an intellectual ground shared by the older disciplines,
so that we may say how and to what extent our field is of as well as in
the humanities, how it draws from and adds to them; at the same time to
reflect experience with computers "in the wild"; and to aim at the most
challenging problems, and so the most intellectually rewarding future
now imaginable.

My primary concern here is, as Confucius almost said, that we use the
correct word for the activity we share lest our practice go awry for
want of understanding (Analects 13.3). Several words are on offer. By
what might be called a moral philology I examine them, arguing for the
most popular of these, "modeling." The nominal form, "model", is of
course very useful and even more popular, but for reasons I will adduce,
its primary virtue is that properly defined it defaults to the present
participle, its semantic lemma. Before getting to the philology I
discuss modeling in the light of the available literature and then
consider the strong and learned complaints about the term.

Background
==========

Let me begin with provisional definitions1. By "modeling" I mean the
heuristic process of constructing and manipulating models', a "model" I
take to be either a representation of something for purposes of study,
or a design for realizing something new. These two senses follow
Clifford Geertz's analytic distinction between a denotative "model of"
such as a grammar describing the features of a language, and an
exemplary "model for" such as an architectural plan
\[\@geertz\_clifford\_clifford\_1973, 93\] 2. In both cases, as the
literature consistently emphasizes, a model is by nature a simplified
and therefore fictional or idealized representation, often taking quite
a rough-and-ready form: hence the term "tinker toy" model from physics,
accurately suggesting play, relative crudity, and heuristic purpose
(Cartwright 1983, 158). By nature modeling defines a ternary
relationship in which it mediates epistemologically, between modeler and
modeled, researcher and data or theory and the world (Morgan and
Morrison 1999). Since modeling is fundamentally relational, the same
object may in different contexts play either role: thus, e.g., the
grammar may function prescriptively, as a model for correct usage, the
architectural plan descriptively, as a model of an existing style. The
distinction also reaches its vanishing point in the convergent purposes
of modeling: the model of exists to tell us that we do not know, the
model for to give us what we do not yet have. Models realize.

Perhaps the first question to ask is what such a process has to do with
computing, since as the examples suggest neither of the two senses of
"model" assumes it unless the definition is further qualified. In
history, for example, Gordon Leff has argued that models have always
been implicit in scholarly practice (Leff 1972). Leff cites, e.g., the
historic-graphical notion of "epoch", but any well-articulated idea
would qualify as a model of its subject. Nevertheless, Leff notes that
as M. I. Finley said in Ancient History: Evidence and Models,
"model-construction is rare among all but economic historians"; Finley
recommends Max Weber's parallel concept of "ideal types", which
"expresses clearly the nature and function of models in historical
inquiry" (1986: 60f). Explicit model-construction is still rare in
mainstream humanities scholarship. Even for non-computational research
in the social sciences, it is more common, as Finley's demarcation
suggests. For example, political schemes by nature model for a better or
at least different world, even if like Marx's historiography they begin
as models of it; delineating them as models is the scholar's obvious
work (Mironesco 2002). Nevertheless, outside computationally affected
scholarly practice Marvin Minsky's simple, straightforward definition
remains alien in style and in thought: "To an observer B, an object A\*
is a model of an object A to the extent that B can use A\* to answer
questions that interest him about A" (Minsky 1965).

A strong temptation for us here is to dismiss the residual alienness of
Minsky's formulation and to accept, as we have accepted computing, the
reified, explicit "model" of Minsky's definition as what we really have
been doing all along. This would, however, be a serious error. As with
the relationship of hypertext to earlier ways of referring (McCarty
2002), the new form of expression, with its vocabulary and tools, means
an altered way of thinking. A historical imagination is required to see
what this means.

Two effects of computing make the distinction between "idea" or other
sort of mental construct on the one hand, and on the other "model" in
the sense we require: first, the demand for computational tractability,
i.e., for complete explicitness and absolute consistency; second, the
manipulability that a computational representation provides.

The first effects a sea-change by forcing us to confront the radical
difference between what we know and what we can specify computationally,
leading to the epistemological question of how we know what we know. On
the one hand, as Michael Polanyi observed, "we can know more than we can
tell" (1966: 4--5). Computational form, which accepts only that which
can be told explicitly and precisely, is thus radically inadequate for
representing the full range of knowledge -- hence useful for isolating
the tacit or inchoate kinds. On the other hand, we need to trust what we
somehow know, at least provisionally, in order not to lose all that goes
without saying or cannot be said in computational form.

Take, for example, knowledge one might have of a particular thematic
concentration in a deeply familiar work of literature. In modeling one
begins by privileging this knowledge, however wrong it might later turn
out to be, then building a computational representation of it, e.g., by
specifying a structured vocabulary of word-forms in a text-analysis
tool. In the initial stages of use, this model would be almost certain
to reveal trivial errors of omission and commission. Gradually, however,
through perfective iteration trivial error is replaced by meaningful
surprise. There are in general two ways in which a model may violate
expectations and so surprise us: either by a success we cannot explain,
e.g., finding an occurrence where it should not be; or by a likewise
inexplicable failure, e.g., not finding one where it is otherwise
clearly present. In both cases modeling problematizes. As a tool of
research, then, modeling succeeds intellectually when it results in
failure, either directly within the model itself or indirectly through
ideas it shows to be inadequate. This failure, in the sense of
expectations violated, is, as we will see, fundamental to modeling.

The second quality of "model" that distinguishes it from "idea" is
manipulability, i.e., the capability of being handled, managed, worked,
or treated by manual and, by extension, any mechanical means (OED: la.).
Change is common to both models and ideas, but at greater or lesser
metaphorical distance, "model" denotes a concrete, articulated plan
inviting the etymological sense of action-by-hand (L. manus) in
response. Manipulation in turn requires something that can be handled
(physical objects, diagrams, or symbols of a formal language) -- and a
time-frame sufficiently brief that the emphasis falls on the process
rather than its product. In other words, the modeling system must be
interactive. Manipulable objects from the physical to the metaphorical
have characterized mathematics, engineering, the physical sciences, and
the arts ab wo, but with exceptions the necessary time-frame, allowing
for interactivity, has been possible only with computing. With its
advent, Minsky has noted, models could be "conceived, tested, and
discarded in days or weeks instead of years" (1991). Computing met
research easily in fields where modeling was already an explicit method
because, Brian Cantwell Smith has pointed out, models are fundamental to
computing: to do anything useful at all a computer must have a model of
something, real or imaginary, in software. But in the context of
computing, models per se are not the point. What distinguishes computers
from other kinds of machines, Smith notes, is that "they run by
manipulating representations, and representations are always formulated
in terms of models" (Smith 1995, 460).

In other words, computational models, however finely perfected, are
better understood as temporary states in a process of coming to know
rather than fixed structures of knowledge. It is of course possible to
argue ideologically, as some still do, that we are converging on and
will achieve such structures,3 but in any case these structures would
not then be models and would no longer have reason to exist in software.
(Note that the history of computing is the story of ever more complex
and extensive software, not less, despite the fact that implementations
in hardware are faster and can be cheaper.) For the moment and the
foreseeable future, then, computers are essentially modeling machines,
not knowledge jukeboxes. To think of them as the latter is profoundly to
misunderstand human knowledge -- and so to constrict it to the narrow
scope of the achievably mechanical.

In analytical terms, as I have suggested, modeling has two phases:
first, construction; second, manipulation. Examples come readily to mind
from ordinary technical practice, e.g., building a relational database,
then querying the data thus shaped to explore emergent patterns. As
experience with databases shows, the two phases often blur into each
other especially in the early stages when use uncovers faults or
suggests improvements that direct redesign. A model 0/and a model for
may be distinct types -- because in our terms they are fixed objects.
But modeling of something readily turns into modeling for better or more
detailed knowledge of it; similarly, the knowledge gained from realizing
a model for something feeds or can feed into an improved version. This
characteristic blurring of design into use and use into (re)design is
what denies modeling of any sense of closure. Modeling for, Utopian by
definition, is denied it in any case.

Learned Complaints
==================

So far so good -- but at the cost of averting our gaze from the problems
with the word "model." Indeed, the extensive and growing literature on
the topic may seem adrift in a hopeless muddle. "I know of no model of a
model", physicist H. J. Groenewold declared many years ago (1960: 98).
The philosopher Peter Achinstein has warned us away even from attempting
a systematic theory (1968: 203). The word itself is indeed astonishingly
polysemous -- or promiscuous, as Nelson Goodman puts it. "Model", he
complains, can be used to denote "almost anything from a naked blonde to
a quadratic equation" (1976: 171). Nevertheless, the word is often used
as if its semantic complexity either did not exist or could be safely
ignored. The muddle of partly overlapping, partly contradictory senses
is proof enough that we ignore it at our peril. Nor can we simply avoid
the problem by dismissing "model" altogether, as Goodman and others
recommend, without (as I will argue) hobbling our ability to understand
inter alia those aspects of computing most important to research -- one
might even say, as I do, its essence. Despite several other, supposedly
less confusing terms on offer, the word remains stubbornly popular in
the literature of the social and physical sciences, the history and
philosophy of science, cognitive science, artificial intelligence, and
related areas.

Theoretical physicist John Ziman and philosopher Stephen Toulmin, for
example, recommend "map" on the basis of its conceptual clarity and
fitness for describing the relationship between theoretical knowledge
and reality (Ziman 2000, 126--38, 147--50). Goodman would have us
collapse modeling into diagramming, which he thinks less troublesome
(1976: 171--3). But preference needs to be based on more than such
criteria; "map", for example, serves experiment much less well than
theory, as I will show. We require a close and careful look at the
semantic fields of all major alternatives, including "map", for their
disjunctions and overlaps. We need to scrutinize each of these, asking
what does it denote and connote that the others do not, and vice versa?
What do all have in common? What are their individual tendencies of
mind, and which of these best suits computing as we are learning to
conceive it?

Philological Analysis of Related Terms
======================================

So far I have used the term "model" as the default, partly for purposes
of convenience, partly because, as I argue, it is right for the job. To
answer the learned criticisms and further clarify our topic, however, I
propose to question it by comparison against the major alternatives:
"analogy", "representation", "diagram", "map", "simulation", and
"experiment." As we have seen, the two decisive criteria are that the
thing named by the chosen term be computationally tractable and
manipulable. Tractability in turn requires complete explicitness and
absolute consistency; manipulability resolves into mechanical action and
interactivity. Hence the term must denote a continual process of coming
to know, not an achievement but an approximation. As I have argued, it
is from the difference between the approximation and the reality
approximated -- which ultimately for the humanities is our humanly known
apprehension of that reality -- that we learn.

For each of the alternative terms I ask whether and to what degree the
word normally denotes a dynamic process and whether it refers to a
concrete, i.e. manipulable, form -- the requirements of anything whose
function is fulfilled through being changed. Corresponding to the two
senses of "model" I identified earlier, the denotative model of and the
exemplary model for, I also ask whether each word tends to the mimetic
(imitation) or proleptic (anticipation). The distinction helps in
determining whether the action denoted by a term may be said to be
bounded, either by a fixed form, as is the case with "analogy", or by an
inherent tendency to reach a definitive or satisfactory conclusion, as
in "representation."

Thus bringing "model" into focus against the semantic background of
these other terms will show that the problem has not so much been too
many meanings for "model" as use without regard to any of them, often as
if the sense of it simply goes without saying. It doesn't. But perhaps
the most important lesson we learn from seeing the word in the context
of its synonym set is not the range and variety of its meanings; rather,
again, its strongly dynamic potential. Apart from the popularity of
"model" taken at face-value, the word would have little to recommend it
(and, as the complainers say, much against it) but for the open-ended
present-participial strength of "modeling."4 Indeed, the manifest
confusion in the literature on the topic may be primarily due to a
mistaken preference for the noun -- as if getting a model right, and so
promoting it to the status of theory, were the point. Modeling has an
entirely different role to play. There are several better terms if what
one wants is to name a stable conceptualization.


