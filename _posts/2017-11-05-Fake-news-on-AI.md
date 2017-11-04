---
layout: post
title: Dangers of AI and Fake News about it
---

__[Česká verze příspěvku](/2017/05/29/Fake-news-o-AI.html)__

While reading news stories about research or products involving deep learning, I
get often surprised how inaccurate and misleading the news stories are. It is
probably a problem of almost all expert fields which happen to appear in media,
luckily they do not bother me as much as AI.

News stories compete the get our attention in a world with so many things to
do. The news story needs to win the never-ending fight for your attention with
your work, Facebook posts, friends, family, books you want to read—and that is
not an easy task at all. Media scientists claim the news must satisfy some
criteria to even get chance to attract the readers' attention, these are called
the [news values](https://en.wikipedia.org/wiki/News_values).  In case of
technology news these are in particular cultural proximity, unambiguity,
personalization (narrating as actions of concrete person).

Obviously, the news must be simplified and put in a shape that fits the news
values. This why the media tend to avoid complicated technical terminology with
something more familiar to the readers—in this case the terminology often comes
from science fiction literature.

Unspoken connections between emerging technologies and sci-fi genre of course
make the news stories more attractive and make the technologies more popular
among the public. On the other hand, it raises false expectations both in terms
of use and possible misuse of the technologies.  Public discussion is
misdirected towards hypothetical risks and overlooks the real ones. Sci-fi
books and movies about AI often re-narrate a myth about the mankind getting
into existential trouble by not reflecting the potential of a recent
technology, showing the same conceit, self-admiration and arrogance as in
stories about [Golem](https://en.wikipedia.org/wiki/Golem), [doctor
Faust](https://en.wikipedia.org/wiki/Faust) or [doctor
Frankenstein](https://en.wikipedia.org/wiki/Frankenstein) (have you ever notice
how often the bad guys have academic degrees?).

In this post, I would like to discuss some of these misconceptions and
highlight what are the main risks these emerging technologies pose.

# Google's Machine Translation Developed its Own Language

At the beginning of this year, Google published a study showing how its neural
machine translation model that is used in Google Translate can be modified in
such a way that a single model is capable to translate between multiple
language pairs, including language pairs that were never seen during the
training. This can be seen on a scheme from [Google Research
Blog](https://research.googleblog.com/2016/11/zero-shot-translation-with-googles.html).

![Google's Zero-Shot Translation](/assets/google_zero_shot.gif)

If this worked, it would be a major advance in machine translation, because
nowadays, we need a separate model for every single language pair. However,
this did not happen.  Although, the results are interesting from the
theoretical perspective, the performance of such models is by large margin
worse than what are users of Google Translate used to. In fact, they more
resemble attempts for machine translation from the early days of its research.

Some people called the common input representation the models had to learn as
_interlingua_ which is a hypothetical common meaning representation that should
be the same for all the languages, an ultimate analysis of a sentence. This
news has been reported even by the most read technology news servers:

* [Wired.com, 23.11. 2017: Google's AI just created its own universal 'language'](http://www.wired.co.uk/article/google-ai-language-create)

* [TechCruch.com, 22.11. 2017: Google’s AI translation tool seems to have invented its own secret internal language](https://techcrunch.com/2016/11/22/googles-ai-translation-tool-seems-to-have-invented-its-own-secret-internal-language/)

The articles not only do not mention that the translation was useless for any
practical purposes, but they also make a false impression that the intermediate
representation that the system uses is something that can be used a language.
This by the way says that current neural networks are so intelligent that they
can not only use human language, but they can invent new, presumably better
languages. In human world, this is an ability that we would attribute to an
autistic genius.  In fact, the representations the system uses are tables with
thousands of real numbers for which we have no direct interpretation. It also
has none of the properties people usually attribute to languages.

# Facebook's AI Grew out of Control, so they Had To Stop It

One of the weaknesses of current models for natural language processing is that
they model only _how does the language look like_. Although language can have
various uses, it mostly used when we to communicate something to someone else:
entertain someone, make someone angry, tell the world what is the right thing
to do or buy a postage stamp. For machine translation, it might enough to teach
the model how does a sentence in a target look like for a given source
sentence. Nevertheless, if we wanted to create a program that negotiates with
someone about something, a program that intentionally follows the goal you want
it to achieve, trying to simulate what people do in similar situation does not
like a good strategy. Obviously, you need to know what you want to achieve in
order to achieve it.

During the last summer, a research team at Facebook did an experiment whose
goal was exactly this. In the experiments, they trained chatbots which were
supposed to negotiate with each other about exchanging hats, balls and book.
They used the same principle as was used for instance while training the
AlphaGo system for playing the game of Go. The systems were given some prior
knowledge how to negotiate and they were improving their negotiation skills by
constantly communicating with each other. AS a result, the system learned to
negotiate very efficiently with each other. On the other hand, the code they
have developed for that did not resemble English at all.

The experiment got surprisingly high media coverage. Most of the news stories
were telling that Facebook had done an experiment with artificial intelligence
that had got out of control and therefore they had to stop it.

* [Forbes.com, 31.7. 2017: Facebook AI Creates Its Own Language In Creepy Preview Of Our Potential Future ](https://www.forbes.com/sites/tonybradley/2017/07/31/facebook-ai-creates-its-own-language-in-creepy-preview-of-our-potential-future)

* [Independent.co.uk: Facebook's Artificial Intelligence Robots Shut Down after they Start Talking to each other in their own language](http://www.independent.co.uk/life-style/gadgets-and-tech/news/facebook-artificial-intelligence-ai-chatbot-new-language-research-openai-google-a7869706.html)

* [Mirror.co.uk: Robot intelligence is dangerous: Expert's warning after Facebook AI develop their own language](http://www.mirror.co.uk/tech/robot-intelligence-dangerous-experts-warning-10908711)

* [Business Insider: Facebooks's AI accidentally created its own language](http://uk.businessinsider.com/facebook-chat-bots-created-their-own-language-2017-6?r=US&IR=T)

At this time, it was the technology news servers that tried to calm down and
explain the exaggerate news from other media:

* [Wired.com, 1.8. 2017: No, Facebook’s chatbots will not take over the world](https://www.wired.com/story/facebooks-chatbots-will-not-take-over-the-world/)

* [Gizmodo, 31.7. 2017: No, Facebook Did Not Panic and Shut Down an AI Program That Was Getting Dangerously Smart](https://gizmodo.com/no-facebook-did-not-panic-and-shut-down-an-ai-program-1797414922)

If we think of it more deeply, it is actually no surprise that the code the
systems had developed was totally different from any language. Human language
is not probably the most efficient code for negotiating about hats, balls and
books, but it has many other fascinating properties: we can write poems in it,
tell jokes, etc. Facebook stopped the experiment not because it was dangerous,
but because it already delivered results they wanted and it was useless for any
practical use.

# Problems with News like this

The way media talk about AI technologies (even the usage of the term AI, what
will say when some will develop a really intelligent intelligence?!)
intentionally resembles the way AI is depicted in the sci-fi literature and
movies. This might be what makes the stories more attractive. The problem is
that while talking about the potential risks of AI, the sci-fi
conceptualization tends to make us think about sci-fi risks. What comes to our
minds are technology getting out of control eventually exterminating humanity
or a supervillain using the emerging technology to conquer the world. The risks
are in fact earthbound well-known problems that has been here since ever:
criminality, power struggle and careless way of doing business.

What I would worry the most is criminal abuse.  I can imagine programs crawling
web and finding opportunities for blackmailing people (matching faces from
LinkedIn images with some or wild parties photos).  Collecting information for
various kind of scams is also likely to happen.  Recently, Stanford university
researchers published a method for estimating sexual orientation exclusively
from publicly available images. There is no need to say how such a tool can be
used in conservative authoritarian regimes.

The risk are not as fatal as in this though experiment and therefore maybe less
interesting for media, but are based on the same principle. A paper awarded by
the best paper price at the [EMNLP 2017 conference](https://emnlp2017.net)
showed that [deep learning models tend to amplify the
bias](http://aclweb.org/anthology/D17-1319) that is present in the training
data they with. One of the examples they showed, was classification of
activities (who does what) captured on photographs. For instance, the models
said there was a female cooking in the photograph in more that 80% cases even
though it was the case only in 60% of the training instances. We can easily
imagine that the same bias amplification can happen in models banks may use to
estimate clients credibility.

None of these sounds super attractive for a news story, nevertheless there are
real problems, much more real than speculation whether deep learning algorithms
cat take over the world. No, they cannot.