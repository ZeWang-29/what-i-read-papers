American Economic Review 2019, 109(10): 3395–3436
https://doi.org/10.1257/aer.20171829

The Dynamics of Discrimination: Theory and Evidence†

By J. Aislinn Bohren, Alex Imas, and Michael Rosenberg*

We model the dynamics of discrimination and show how its evolution
can identify the underlying source. We test these theoretical predic-
tions  in  a  field  experiment  on  a  large  online  platform  where  users
post  content  that  is  evaluated  by  other  users  on  the  platform.  We
assign posts to accounts that exogenously vary by gender and eval-
uation histories. With no prior evaluations, women face significant
discrimination.  However,  following  a  sequence  of  positive  evalua-
tions,  the  direction  of  discrimination  reverses:  women’s  posts  are
favored over men’s. Interpreting these results through the lens of our
model, this dynamic reversal implies discrimination driven by biased
beliefs.

JEL C93, D83, J16, J71

(

)

)

A  rich  literature  has  documented  discrimination  in  a  wide  range  of  contexts
. These empirical studies have mostly focused on static
Bertrand and Duflo 2017
(
settings: individuals are evaluated based on the quality of a single piece of output
or a single interaction, with no information on prior evaluations in similar contexts.
As prior work has noted, it is difficult to identify the underlying source of discrim-
ination from such static settings, as different sources generate the same patterns of
. In this paper, we develop a theoretical
observable behavior
framework to show how the dynamics of discrimination can be used to identify its
underlying source, and test these predictions in a field experiment on a large online
platform.

Fang and Moro 2011

)

(

Consider a setting where individuals repeatedly perform tasks that generate out-
put, and in the process, produce an observable history of evaluations on these tasks.
For example, a man and a woman are employed at a firm and are promoted based on

)

)

; Rosenberg: CarGurus, 2 Canal Park, Cambridge, MA 02141

; Imas: Carnegie Mellon University, 5000 Forbes Avenue, Pittsburgh, PA 15213

* Bohren:  University  of  Pennsylvania,  133  South  36th  Street,  Philadelphia,  PA  19104

email:  abohren@
email: aimas@
sas.upenn.edu
(
email: rosenberg.michael.m@
andrew.cmu.edu
. Stefano DellaVigna was the coeditor for this article. We thank Nageeb Ali, Linda Babcock, Michael
gmail.com
)
Callen,  Hanming  Fang,  Uri  Gneezy,  Polina  Imas,  Nicola  Gennaioli,  Gregor  Jarosch,  Emir  Kamenica,  Gene
Kucher, George Loewenstein, Kristof Madarasz, Craig McIntosh, Margaret Meyer, Siqi Pan, Sally Sadoff, Lise
Vesterlund,  Leeat Yariv,  and  seminar  and  conference  participants  for  helpful  comments.  We  thank  Mustafa
Dogan, Daniel Hauser, Conrad Kosowski, Catherine Lillis, Suneil Parimoo, Jaesung Son, and Lucia Zhang for
excellent research assistance. Finally, we would like to thank the team at the online forum for helpful and illu-
minating discussions, and for providing us with the data for our analyses. The project received IRB approval at
Carnegie Mellon and University of Pennsylvania. The experiment was pre-registered in the AEA RCT Registry
. The authors declare that they have no relevant or material financial interests that relate
AEARCTR-0000950
(
to the research described in this paper.

)

(

(

† Go  to  https://doi.org/10.1257/aer.20171829  to  visit  the  article  page  for  additional  materials  and  author

disclosure statements.

3395

3396

how managers evaluate their output. Their past promotions and performance evalu-
ations correspond to the history of evaluations. Alternatively, workers contribute to
crowdsourcing projects on a platform, such as GitHub. Each worker has an observ-
able reputation score based on prior evaluations of his or her contributions. In such
settings, when workers are starting out and lack evaluations of prior performance,
initial discrimination occurs if a female worker’s output is less likely to earn a pro-
motion or receive a positive evaluation than a male’s, despite the appearance of sim-
ilar quality. Suppose new workers continue producing output, and receive similar
sequences of evaluations. Does discrimination persist in this dynamic setting, is it
mitigated, or does it even reverse?

)

(

The answer to this question depends critically on the underlying source of dis-
crimination.  If  the  source  is  belief-based—for  example,  the  quality  of  output
is  imperfectly  observed  and  evaluators  believe  that  on  average,  men  have  higher
abilities than women—then observing prior evaluations will reduce discrimination
against women, relative to men with similar evaluations. This dynamic effect oper-
ates  through  two  channels.  First,  prior  evaluations  provide  signals  of  a  worker’s
ability, which reduces the impact of perceived group statistics
e.g., beliefs about
 on how the worker’s subsequent output is evaluated.1 This mitigates
average ability
discrimination between males and females with similar evaluation histories. Second,
and particular to a social learning setting, the informational content of these signals
is endogenously determined by the behavior of prior evaluators. When initial beliefs
favor men, to overcome this disparity, a woman needs to produce higher quality out-
put than a man to receive a similar evaluation: for example, to be promoted or have
her output accepted. This speeds up the mitigation of discrimination for evaluators
who are aware of the higher standard for women. These evaluators may even come
to believe that the woman is of higher ability than a man with a similar evaluation
history, thereby favoring her output over the man’s and reversing the direction of
discrimination in subsequent periods. In fact, observing a reversal can help disentan-
gle whether evaluators’ models are correct or misspecified; we show theoretically
that  a  reversal  provides  evidence  for  bias.  In  contrast  to  belief-based  sources,  if
discrimination is caused by a taste or preference against rewarding or interacting
with women
, then a woman who receives a similar sequence of eval-
(
uations to a man will continue to face discrimination in future periods.

Becker 1957

)

Our theoretical framework formalizes the relationship between the dynamic pat-
tern  of  discrimination,  which  is  based  on  observable  evaluations,  and  the  sources
of  discrimination,  which  are  unobservable  and  depend  on  underlying  preferences
and beliefs. The literature on belief-based sources has generally focused on correct
, where evaluators are partial toward a group based
e.g., rational expectations
beliefs
)
(
on true differences in the underlying distributions of the relevant attribute
Fang and
(
Moro  2011;  Phelps  1972;  Altonji  and  Pierret  2001;  Knowles,  Persico,  and  Todd
. However, recent research has demonstrated that systematic biases in judgment
2001
)
Schwartzstein  2014;
can  lead  to  incorrect  stereotypes  against  a  particular  group
(

1 This  is  the  channel  typically  considered  in  the  literature  on  accurate  statistical  discrimination,  i.e.,  belief-
based discrimination with correct beliefs
. The discrimination literature in social
e.g., Altonji and Pierret 2001
psychology also discusses the role of individual-specific information in reducing reliance on using group statistics
for judgment

(

)

.

see Fiske 1998 for review
(

)

THE AMERICAN ECONOMIC REVIEWOCTOBER 20193397

i

)

(

)

(

)

(

iii

 belief-based with correct beliefs,

. Therefore, we allow for three poten-
Fryer and Jackson 2008; Bordalo et al. 2016
 belief-based with incorrect,
ii
tial sources:
)
biased beliefs, and
 preference-based. We show that these sources make con-
trasting dynamic predictions. When discrimination is based on common knowledge
of correct beliefs, then observing similar sequences of evaluations for a man and
a woman will mitigate discrimination, but will never lead to a reversal. Therefore,
observing  a  dynamic  reversal  provides  evidence  for  a  belief-based  source  with
bias, since it is also inconsistent with standard preference-based sources. We also
illustrate how one form of bias, where some evaluators hold incorrect stereotypes
against a group and other evaluators are aware of these stereotypes, can lead to a
dynamic reversal.

(

Fiske et al. 1991

Our  framework  also  formalizes  how  a  second  informational  channel,  the  level
of subjectivity in evaluation
, modeled as the precision in signals
of  quality,  provides  further  evidence  to  disentangle  the  source  of  discrimination.
Specifically,  decreasing  the  subjectivity  of  evaluations  will  mitigate  belief-based
discrimination, as beliefs about group statistics play a smaller role in assessing qual-
ity when signals of quality are more precise. But it will not affect preference-based
discrimination, which will persist even if quality is perfectly observable. As we later
discuss, identifying the underlying source of discrimination has significant implica-
tions for policy and welfare.

)

We test these theoretical predictions using a field experiment on a large online
Q&A  forum.  The  forum  is  a  prominent  resource  for  students  and  researchers
in  STEM  fields—it  has  nearly  350,000  users,  and  belongs  to  a  family  of  Q&A
forums that has over 3 million questions asked and 4 million answers posted per
year—which  makes  documenting  the  existence  and  source  of  gender  discrimi-
nation  in  this  setting  particularly  important.  Users  post  mathematics  questions
or  answers,  and  these  posts  are  evaluated,  voted  up  or  down,  by  other  users  on
the site. A user’s reputation provides a summary statistic of evaluations of his or
her past posts: higher reputation corresponds to more positive and fewer negative
votes. Importantly, reputation is publicly observable and highly visible. Both the
username and the level of reputation are prominently displayed adjacent to any
post. Since reputation  is generated by  prior evaluations, this setting mirrors the
social learning in our theoretical framework. Reputation is also valuable: it can
be  used  as  currency  to  pay  other  users  for  providing  answers  and  it  promotes
users to higher ranks on the forum, opening the door to additional privileges. This
includes privileges to “supervise” other users: for example, to edit, flag, and close
other users’ posts. Similar to promotion decisions within a firm, evaluations are
consequential because reputation gives users greater influence over the evaluators.
Therefore,  the  link  between  evaluations  and  advancement  on  the  forum  mirrors
many labor market settings.

In our experiment, we posted original mathematics questions on created accounts
that exogenously vary in the gender of the username and the reputation of the user.
Our setting is well suited for exploring the dynamics of discrimination because we
are  able  to  exogenously  vary  the  evaluation  histories  of  users,  as  summarized  by
their publicly observable reputations. We posted one-half of the questions to nov-
ice accounts that did not have prior evaluations. We manually built the reputations
of the remaining accounts by posting content until the reputations reached the top

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 103398

twenty-fifth percentile on the forum. We then randomly reassigned the gender of the
username to avoid endogeneity issues and ensure that the underlying informational
content of reputation is the same for both genders. Finally, we posted the remaining
questions  to  these  advanced  accounts.  We  compare  the  pattern  of  discrimination
between novice and advanced question posts to test the dynamic predictions of the
different sources of discrimination.

)

We also posted answers to other users’ posts from a second set of novice accounts
that exogenously vary the gender of the username. This allows us to test the compar-
ative static on how the level of subjectivity involved in judging posts
e.g., the preci-
(
 affects discrimination. While the forum’s guidelines for voting on
sion of the signal
whether the question is interesting,
questions are based on fairly subjective criteria
(
useful, or well-researched
whether
)
the answer is correct or not
. If the source is preference-based, this distinction will
not  affect  discrimination:  our  model  predicts  similar  levels  of  discrimination  for
both question and answer posts. In contrast, if discrimination is belief-based, then
our model predicts that reducing subjectivity will mitigate it: answer posts will face
less discrimination than question posts.2

, the guideline for voting on answers is clear-cut
(

)

We measure discrimination as the difference in reputation earned or net votes
on posts by accounts with male versus female usernames. We find no significant
discrimination  on  answer  posts:  answers  posted  by  females  with  no  prior  eval-
uations earned a similar amount of reputation and received a similar number of
positive votes as answers posted by males with no evaluations. In contrast, we find
that females face significant initial discrimination when the judgment of quality
is more subjective: questions posted to female accounts with no prior evaluations
are  evaluated  less  favorably,  earning  less  reputation  and  fewer  positive  votes,
than  questions  posted  to  similar  male  accounts.  Directly  comparing  questions
and answers produces a significant interaction, indicating greater discrimination
against females when judgments of quality are more subjective. This is consistent
with  belief-based  but  not  preference-based  discrimination. We  also  find  signifi-
cant discrimination on questions posted to advanced accounts, but the direction
of  discrimination  reverses:  questions  posted  to  advanced  female  accounts  earn
more  reputation  than  those  posted  by  similarly  advanced  males.  This  produces
a significant interaction effect between the user’s rank on the forum
Novice or
  and  gender.  Interpreting  these  results  through  the  lens  of  our  model
Advanced
suggests that initial discrimination is belief-based, with bias playing a role in the
evaluation process.

(

)

In addition to our experimental results, we exploit two additional data sources: a
proprietary dataset that contains additional information about the users who evalu-
ated the content from our experiment, and a large observational dataset of all posts
on the forum. We used these datasets to run additional robustness tests and to rule

2 An evaluator who has a preference against women but does not want to appear discriminatory, either to him-
self or others, may also discriminate less on objective quality dimensions, as such discrimination is more obvious
. Two features of our experimental setting suggest that
e.g., moral wiggle room
(
this phenomenon may be less likely to emerge:
 evaluators are anonymous, removing the motivation to signal
to others; and
 discrimination mostly occurs along the margin of choosing whether to upvote or not evaluate
)
a post. We observe few downvotes, and moral wiggle room is typically conceptualized as an avoidance of salient
negative actions.

Dana, Weber, and Kuang 2007

ii
(

))

(

(

)

i

THE AMERICAN ECONOMIC REVIEWOCTOBER 20193399

out other potential explanations for the observed reversal, such as gender differences
in attrition or the variance of ability. We also compare discrimination by type of post
and reputation in the observational data. We find analogous patterns to the experi-
ment, including both the dynamic reversal between questions posted by novice and
advanced users and the lack of discrimination for answers.

The findings presented here highlight the importance of studying discrimination
in dynamic settings, as discrimination in favor of a certain group, or a lack thereof,
at any given stage can either be a function of or precursor to discrimination against
that same group at a different stage. Both in academic and popular discourse, a
common argument used to illustrate the lack of discrimination against a group is
to point to individuals from that group who have made it to positions of promi-
nence. Our theoretical framework and empirical evidence highlight the flaw of this
argument: if individuals are aware that members of a group face discrimination
at an earlier stage, there may be Bayesian foundations for favoring members of
that group at later stages. For example, in a much-discussed paper, Williams and
Ceci
 find that accomplished female academics in STEM fields are
(
favored over male academics. The authors state that “these results suggest it is a
propitious  time  for  women  launching  careers  in  academic  science.”  In  contrast,
other work has found significant discrimination against female students in STEM
. While these
Reuben, Sapienza, and Zingales 2014; Moss-Racusin et al. 2012
(
sets  of  findings  appear  contradictory,  our  results  suggest  that  discrimination  in
favor of accomplished female professors may actually be a function of discrimi-
nation against women earlier in the pipeline.

2015, p. 5361

)

)

)

Our conceptual and experimental framework can be applied to many other labor
market  settings.  Settings  where  individuals  offer  a  product  and  can  be  identified
by their gender and prior history of evaluations are becoming progressively more
widespread  and  economically  important.  Stack  Exchange,  GitHub,  TaskRabbit,
Upwork, and Airbnb are just a few examples of such platforms. Our framework is
also relevant for settings in which prior work has found reversals of discrimination
between the hiring and promotion stages within a firm, and it provides a possible
explanation  for  the  “female  leadership  premium”
  that  has
)
been documented in the management literature
see the Related Literature section
for further discussion

again,  within  a  firm

(

(

.

Our results are also useful for assessing the welfare consequences of discrimi-
nation. While the welfare implications of discrimination driven by preferences or
correct  beliefs  are  unclear,  the  welfare  implications  of  discrimination  caused  by
biased beliefs are more straightforward: in our setting, biased beliefs lead to dis-
torted evaluations. Even if a discrimination reversal occurs, so that women even-
tually receive higher evaluations than men with similar evaluation histories, these
women still receive lower evaluations than men with similar output quality histories.
In other words, the reversal does not offset initial discrimination: a woman who is
favored over a man with a similar evaluation history should receive an even higher
evaluation than she does, given correct beliefs about her expected ability. Perhaps
even more importantly, women may inefficiently stagnate at lower stages than men
with  similar  abilities  due  to  initial  discrimination. That  is,  women  and  men  with
similar output histories will not achieve the same level of success: the women will
be systematically underrated. Therefore, hiring and promotion decisions based on

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 103400

these evaluations will be suboptimal, particularly when future evaluators are also
biased or are not aware of the bias of prior evaluators.3

Finally, our results highlight the importance of considering the dynamic impact of
interventions that aim to reduce discrimination, particularly in regards to how these
interventions impact beliefs. For example, evidence suggests that individuals sys-
tematically overestimate the prevalence of affirmative action policies and the extent
. An interven-
to which they lower evaluation standards
(
tion that leads to perceived lenient standards at one stage will impact assessments at
later stages, and can even lead to greater subsequent discrimination. This highlights
the importance of accurately informing the population who evaluates members of a
target group about the scope of such interventions.

Kravitz and Platania 1993

)

)

)

)

)

)

)

(

, housing

, ethnicity

,  and  service  markets

)
Gneezy,  List,  and  Price  2012
(

Related Literature.—Discrimination has been documented in a wide range of set-
tings, including hiring
Ewens,
Riach and Rich 2006; Bartoš et al. 2016
(
Tomlin,  and  Wang  2014
.  It
has  also  been  documented  against  group  identities  based  on  race
Bertrand  and
(
Mullainathan 2004; Parsons et al. 2011
Fershtman and Gneezy 2001;
(
Milkman, Akinola, and Chugh 2012
Moss-Racusin et al. 2012; Goldin
 and gender
(
and Rouse 2000
. The few studies that use observational data to attempt to identify
the source of discrimination typically compare the evaluations of a state
for exam-
ple, whether output is accepted or rejected
 to the true underlying value of that state
i.e., whether the output was actually high or low quality
. For example, Knowles,
(
 compare decisions of law enforcement to search a motor
Persico, and Todd
vehicle to the success rate of the search; similarities in success rates across races
led the authors to conclude that higher search rates for African American drivers are
due to statistical rather than preference-based discrimination
see, for similar tests,
. In recent work, Sarsons
Anwar and Fang 2006 and Arnold, Dobbie, and Yang 2018
)
 uses an event study approach for matched samples of surgeons to explore
2017
(
)
belief-based  gender  discrimination  in  physician  referrals.  She  concludes  that  the
observed pattern of gender discrimination is not consistent with Bayesian learning
with respect to accurate beliefs about the distribution of surgeon ability. However,
in  many  observational  settings,  it  is  difficult  or  impossible  to  construct  matched
samples or to observe the true value of the underlying state at an individual level.
Further, observational data often face endogeneity issues that preclude the causal
identification of discrimination.

2001

(

(

)

(

)

Due to endogeneity issues, many researchers have employed field experiments to
study discrimination. Field experiments have been successful in causally identify-
ing the incidence of discrimination, but most cannot identify the source of this dis-
crimination
, who
)
documents that minorities receive inferior initial and final offers when bargaining
in a market for sports cards. He supplements these data with a series of artefactual
and framed field experiments to identify the source of this discrimination. Data from

. One notable exception is List

Bertrand and Duflo 2017

2004

(

(

)

3 More  generally,  in  learning  settings  with  no  action  interdependence,  an  individual  with  an  incorrect  belief
about the prior distribution of ability or informational content of evaluations will make suboptimal choices, relative
to an individual with correct beliefs. This contrasts with settings with action interdependence, in which the effect of
incorrect beliefs is ambiguous: when correct beliefs lead to a market failure, it may be possible for incorrect beliefs
to improve the market outcome.

THE AMERICAN ECONOMIC REVIEWOCTOBER 20193401

dictator games, market, and auction experiments provide support for belief-based dis-
crimination, and rule out preference-based sources. This method demonstrates how
eliciting the true value of the underlying state for different groups
e.g., the distribu-
(
 can identify the source of discrimination in a
tion of reservation prices across races
)
static setting. We provide a complementary approach that illustrates how dynamic data
and variation in the subjectivity of judgment can be used to achieve the same goal.

(

)

(

)

)

(

(

1986

2010

1999

1996

Our  findings  shed  light  on  the  mechanism  behind  previously  documented  dis-
;
crimination  reversals.  In  labor  market  settings,  Groot  and  van  den  Brink
)
;  and  Petersen  and  Saporta
;  Lewis
Booth,  Francesconi,  and  Frank
  find  discrimination  against  women  at  the  initial  hiring  stage  for  promot-
2004
(
able  jobs,  but  conditional  on  being  hired,  they  find  that  women  are  more  likely
to be promoted. Rosette and Tost
 document a female leadership premium,
)
showing that in contrast to women at lower levels within an organization, women
in high positions are seen as more effective than men at similar positions.4 In a field
 show that workers are more likely to
2018
experiment, Ayalew, Manian, and Sheth
)
(
follow a man’s advice than a woman’s; however, this result reverses when they are
informed that the woman or man has achieved a high level position in a job outside
of the experiment. In the art market, Bocart, Gertsberg, and Pownall
 docu-
)
ment that while female artists are less likely to transition from primary to secondary
art markets,  those who do command a  4.4 percent premium on artworks sold. In
academia, Mengel, Sauermann, and Zölitz
 find that junior female instructors
(
systematically receive lower teaching evaluations compared to male instructors for
similar courses, but at the senior level, female instructors receive higher evaluations
than male instructors. While these results could be driven by institutional factors,
our theoretical and empirical findings suggest that the reversals may be driven by
belief-based  discrimination  with  bias
.
)
 find that
Consistent with this mechanism, Mengel, Sauermann, and Zölitz
)
initial discrimination against females is higher in courses with math-related content,
where distorted gender stereotypes are more likely to play a role

for  example,  biased  priors  or  stereotypes

Coffman 2014

2018

2019

2019

(

)

(

(

The paper proceeds as follows. Section I presents the theoretical model, Section II
presents the experiment and analysis of observational data, while Section III dis-
cusses the implications for policy and concludes. All proofs are in the Appendix.

.
)

(

I.  A Dynamic Model of Discrimination

We develop a dynamic model of discrimination in which evaluators learn about a
worker’s ability from group identity and past performance, and use this information
to evaluate the quality of the worker’s current output. To mirror our experiment, we
use gender as the group identity in our model and focus on discrimination against
F

emales

ales

.

(

 compared to M
)

(

)

)

(

2017

4 Leslie, Manchester, and Dahm

 argue that this leadership premium extends to perceived potential as
well. In their paper, women who are perceived to be able to rise through the ranks are judged to add more value
to the company than men with similarly high potential; in contrast, low potential women are judged to add less
value than low potential men. Importantly, substantially fewer women are judged as being able to rise through the
ranks than men. Gornall and Strebulaev
 use a field experiment to show that promising female entrepreneurs
(
receive  significantly  more  interested  replies  from  venture  capitalists  than  male  entrepreneurs  pitching  identical
projects. See also Beaman et al.

 for the effect of exposure to female leaders on perceived effectiveness.
)

2019

2009

)

(

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 103402

We first set up the model and formalize the definitions of the underlying belief
and  preference-based  sources  of  discrimination,  then  briefly  comment  on  nota-
ble features of our setting, including how we choose to model belief-based dis-
. In
crimination, incorrect beliefs, and the subjectivity of judgment
Section IB, we characterize how beliefs and preferences impact initial evaluations,
and show that varying the level of subjectivity in judgment can identify whether
.  In
discrimination  is  due  to  preference-  or  belief-based  sources
Section IC, we characterize how discrimination evolves across time. This yields
two main results: Proposition 2 establishes the impossibility of a discrimination
reversal  when  all  evaluators  have  common  knowledge  of  correct  beliefs,  while
Proposition 3 demonstrates how one form of biased beliefs can lead to a reversal.
A reader who prefers to skip the formal presentation of the theory can jump to the
empirics in Section II.

Proposition  1

Section IA

(

(

)

)

A. Model

Worker.—Consider a worker who has observable group identity  g
/ τ a  )
1

  and
}
0 .
 τ a    >
 . Each task has hidden qual-
  is an independent random shock with pre-
1 .  Ability  is  fixed  across  time,  and  higher  ability  generates  higher

unobservable ability  a
The worker completes a sequence of tasks  t
q
ity
 t    =
cision
expected quality.

F,
  and precision

 , with mean
2,

,
 ( μ g
N
0,
 (

 μ g    ∈  ℝ
 …

 , where

 ϵ t    ∼

 +  ϵ t

  ∈   {

 τ ϵ    >

/ τ ϵ  )

  =

  ∼

M

1,

N

a

1

Evaluators.—A set of evaluators assess the worker’s performance. For simplicity,

v
assume that there is one evaluator per task, who reports evaluation
 t    ∈  ℝ

 .

 t   +  η t

v
 t
1  )
−
   of  quality  of  the  current  task,  where
 η t    ∼

Histories and Signals: Before evaluating task  t , the evaluator observes the work-
er’s  gender   g ,  evaluations  on  past  tasks
h
 ,  and
q
N
s
   is  an
signal
 t    =
 (
0 . Lower signal precision reflects
independent random shock with precision
greater  uncertainty  in  quality. This  precision  can  be  interpreted  as  the  amount  of
subjectivity in judgment involved in the evaluation of quality, with lower precision
implying greater subjectivity. We motivate and discuss this interpretation in further
detail in the Discussion of Model.

h
 ,  where
 1    =  ∅
1
0,
/ τ η  )

v
,
 t    =   (
 1
 …

 τ η    >

,

 θ i

Preferences and Beliefs: An evaluator’s type

  determines her preferences and
model of inference, including her subjective belief about the relationship between
gender and ability and her subjective belief about other evaluators’ preferences and
2   from reporting evaluation
v
beliefs. The evaluator receives payoff
−
i
v  on a task of quality  q  from a worker of gender  g , where
c
  is a type-specific taste
  g
i
 ˆ
c
  about
0 . The evaluator has subjective prior belief
parameter. Normalize
    g
  μ
the  average  ability  of  a  worker  of  gender   g . We  allow  for  the  possibility  that  the
evaluator has a misspecified model of the relationship between gender and ability,
in that the evaluator’s subjective belief may differ from the true population average
i
 ˆ
 .
ability,
   ≠   μ g
    g
  μ

An  evaluator  is  partial  toward  men  if  she  favors  male  workers,  either  through
her  subjective  belief  about  the  distribution  of  ability  by  gender,  which  we  refer

i
 ))
  g

c
 −

 −  ((

i
  M

   =

q

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019

to as belief-based partiality, or through preferences, which we refer to as prefer-
ence-based  partiality.  In  the  first  case,  an  evaluator  has  a  “taste”  favoring  male
workers, meaning that she has a disamenity value associated with tasks produced by
female workers.

3403

DEFINITION 1
(
c
ence-based partiality toward men if

Preference-Based Partiality
0 .

i
  F
   >

)

: An evaluator of type

  has prefer-

 θ i

In the second case, the evaluator believes that the average ability of male workers
is higher than the average ability of female workers. Belief-based partiality can be
biased or unbiased, based on whether it coincides with the true population average
for each gender.

DEFINITION  2
i
 ˆ
based partiality toward men if
    M
  μ
i
 ˆ
and
   =   μ F
    F
  μ

:  An  evaluator  of  type
Belief-Based  Partiality
)
i
i
 ˆ
 ˆ
 . This partiality is unbiased if
    M
    F
  μ
   >    μ
 , and otherwise is biased.

 θ i

(

   has  belief-

   =   μ M

Finally, in order to interpret the evaluation history, which consists of the assess-
ments of other evaluators, the evaluator needs a model of other evaluators’ prefer-
ences and beliefs. This is captured by her subjective belief about the distribution over
 ˆ
types,
   i    ∈  Δ (Θ)
π  ∈  Δ (Θ)
  π
denote the true distribution over types. A misspecified model of how others evaluate
workers  is  captured  by  a  subjective  belief  about  the  type  distribution  that  differs
 ˆ
 . We discuss settings this framework can capture
from the true distribution,
   i    ≠  π
  π
in the Discussion of Model.

  denotes the finite set of evaluator types. Let

 , where

Θ

Aggregate  Beliefs:  It  is  straightforward  to  define  aggregate  analogues  of  par-
tiality  with  respect  to  the  average  beliefs  and  preferences  of  evaluators. There  is
i
i
 ˆ
 ˆ
E
E
   and  aggregate
aggregate  belief-based  partiality  toward  men  if
 ]
 π   [  μ
 ]   >
 π   [  μ
    F
    M
i
c
E
0 ,  where  the  expectation  is
preference-based  partiality  toward  men  if
 ]   >
 π   [
  F
taken with respect to the true distribution over types. Aggregate belief-based par-
i
i
 ˆ
 ˆ
E
E
 , and otherwise is biased. It
  and
tiality is unbiased if
 ]   =   μ F
 π   [  μ
 π   [  μ
    F
    M
is possible for individual types to exhibit partiality or bias, but for aggregate prefer-
ences and beliefs to be impartial or unbiased.5

 ]   =   μ M

Belief-Updating: The evaluator learns about the worker’s ability from the evalua-
tion history. Her posterior belief about ability is derived using Bayes’ rule, given her
model of inference. She combines this updated belief about ability with the signal to
learn about the quality of the current task, also using Bayes’ rule to form her poste-
rior belief about quality.

5 For example, suppose each type’s prior belief about average ability is the true mean plus an idiosyncratic error.
This would result in partiality at the individual level, in that some evaluators are partial toward men and others are
partial toward women, but no aggregate partiality.

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 10

3404

Optimal Evaluations: Each evaluator chooses the evaluation that maximizes her
expected payoff with respect to her posterior belief about quality. Suppose an eval-
uator has type

  and let

 θ i

1

(

)

h,

s,

v

 i   (

g
)   ≡

E ˆ
   i   [−   (v
arg max
  v
∈ℝ

 −  (q

c
 −

2
i
 ) )
  g
  |

h,

s,

g]

denote her optimal evaluation conditional on observing history  h  and signal  s  from
E ˆ
a worker of gender  g , where
  denotes the expectation with respect to her model of
   i
inference. Then her optimal evaluation is

)

(

2

g

s,

s,

h,

h,
v
 i   (

E ˆ
q
   i   [
)   =
Discrimination.—Discrimination  is  the  disparate  evaluation  of  workers  based
on  the  group  to  which  the  worker  belongs,  i.e.,  gender,  rather  than  on  individual
attributes, i.e., signal and history. In our framework, gender discrimination occurs
when a male and female worker with the same evaluation history and current signal
receive different evaluations. Let

c
g
]  −

i
  g
 .

 |

3

)

(

h,

D

 i   (

denote the difference between type
ditional on observing history  h  and signal  s , and let  D
the expected difference in evaluations across all types.

F

s,

s,

h,

M

h,
 i   (

v
)  −

v
s
 i   (
)   ≡
 ’s evaluation of a male and female worker con-
  denote

 θ i

)

s

h,
 (

h,
D
E
 π   [
 i   (
)   ≡

s
) ]

)

Discrimination

:  A  woman  faces  discrimination  from  type

DEFINITION  3
h,
D
   if
s
h,
 i   (
)
(
aggregate
faces
(

(
s
)   >
)

0 ,  and  faces  aggregate  discrimination  if   D
 (
 .
s
)
)   <

D
 discrimination if
 i   (
In contrast to partiality, which is a property of the primitives of the model
ences, beliefs

, discrimination is a property of behavior.

h,
D
0
 (
 (

)   <

)   >

h,

s

h,

0

s

   at
 θ i
0 .  A  man

prefer-

(

In this paper, we study whether discrimination reverses between histories.

)

Discrimination Reversal

DEFINITION 4
)
(
tory  h  and signal  s  if there exists a history  h
tion at   (h

′  ⊂
h,
s)   and men face discrimination at
 (

,

′

: A discrimination reversal occurs at his-
h  such that women face discrimina-
s

.6 )

For example, a discrimination reversal occurs if women face initial discrimination
h
v
h
 , while men face discrimination at history
  following
at history
 1    =  ∅
 1  }
 2    =   {
v
 . We also study whether discrimination decreases, for example,
some evaluation
 1
s
 .
between histories or across parameters, which corresponds to a decrease in
) |
|
In the following sections, we explore how the different forms of partiality impact
i.e.,

D
 (
discrimination.  We  use  these  insights  to  illustrate  how  observable  behavior

h,

(

6 Given histories  h

v
  and  h
v
,
,
 m  )
 1
 …
′  =   (
  for all  t
v
v
same first  m  evaluations, i.e.,
  t  ′
 t    =

v
,
  1  ′
  =   (
m .
  ≤

 …

,

v

 , we say  h

  n  ′  )

′  ⊂

h  if  m

  <

n  and the histories have the

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019

 can be used to identify the source of discrimination
)

(

i.e., preferences,

3405

evaluations
beliefs

.

)

Discussion of Model.—Here, we discuss several features of the model and the

types of settings it can capture.

)

(

2018

π ( θ 1  )   =

Misspecified Models of Inference: The setup for the evaluator’s model of infer-
ence builds on the framework of social learning with model misspecification devel-
oped in Bohren and Hauser
. This framework can capture broad classes of
model misspecification, including an incorrect model of the relationship between
ability  and  gender  and  an  incorrect  model  about  other  evaluators’  preferences
or  beliefs.  For  example,  the  setting  where  all  evaluators  have  common  knowl-
edge that they share the same preferences and beliefs is captured by a single type
1 ,  who  correctly  believes  that  all  other  evaluators  are  this  type,
 ,
 θ 1
 ˆ
1 . This  type’s  subjective  belief  about  average  ability  by  gender  may  or
   1   ( θ 1  )   =
  π
may not be correct. We analyze the dynamic behavior in this setting in Proposition 2.
Alternatively, there may be heterogeneity in evaluators. For example, some eval-
uators may use a heuristic to form beliefs about the relationship between ability and
gender, while other evaluators have a correct belief about average ability by gender.
Evaluators who use a heuristic are likely not aware of their bias—otherwise, they
would  correct  for  it—and  believe  that  other  evaluators  form  beliefs  in  a  similar
manner
 or the
. Our framework can model
false consensus effect
))
(
  that has an incorrect subjective belief about average abil-
this setting using a type
ity by gender and an incorrect subjective belief that other evaluators are the same
 ˆ
  has a correct subjective belief about the ability
type,
   1   ( θ 1  )   =
  π
distribution for males and females, and can either accurately anticipate the presence
 ˆ
0 , or
of the biased type,
   2   ( θ 1  )   =  π ( θ 1  )
  π
 ˆ
 . This type
under- or overestimate its frequency,
   2   ( θ 1  )   <  π ( θ 1  )
  π
could also be aware that some evaluators are biased, but not understand the exact
extent of the bias. Importantly, when there is heterogeneity in evaluators’ subjective
beliefs about the relationship between gender and ability, then at least one type has
a misspecified model of inference. We explore the dynamic behavior in this setting
in Proposition 3.

 ˆ
 , be unaware of the biased type,
   2   ( θ 1  )   =
  π

as in the case of the bias blind spot

 ˆ
  or
   2   ( θ 1  )   >  π ( θ 1  )
  π

Ross, Greene, and House 1977

Pronin, Lin, and Ross 2002

1 . The other type

 θ 1

 θ 2

(

)

(

Belief-Based Discrimination: Theories of belief-based discrimination have typ-
ically focused on rational, or statistical, discrimination, where evaluators hold cor-
rect  beliefs  about  aggregate  group  differences.  These  models  fall  into  two  broad
categories that differ primarily in how group differences in beliefs arise, whether
i
)
(
group differences are exogenous and discrimination is due to imperfect information
 group differences are “self-fulfilling” and discrimination is an
, or
Phelps 1972
(
(
.7 In the first class of models, evaluators hold prior
equilibrium effect
(
beliefs  about  workers’  abilities  that  differ  by  group  identity  and  use  these  group
Altonji and Pierret 2001, Aigner and Cain 1977,
statistics to infer individual ability
(

ii
)
Arrow 1973

)

)

7 See Fang and Moro

2011

(

)

 for a more thorough review of this literature.

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 10

3406

)

Lundberg and Startz 1983
. Our model with correctly specified evaluators falls into
this class. In the second class of models, ex ante identical workers decide whether
to engage in costly and unobservable skill acquisition. Discrimination arises when
workers from different groups coordinate on equilibria with different levels of skill
acquisition
.  In  contrast  to  the  first  class  of
models, there are also always equilibria in which both men and women acquire the
same level of skill and evaluators treat them identically.

Coate  and  Loury  1993,  Fryer  2007

)

(

see Bohren et al. 2019 for evidence
(

Belief-based discrimination can also arise from systematically incorrect, or biased,
beliefs. Here, an evaluator engages in inaccurate statistical discrimination because
her decision is based on a misspecified model of group differences in the distributions
. Several models provide microfoun-
of ability
)
dations  for  how  such  biased  beliefs  about  group  differences  can  arise  and  persist.
Evaluators may form biased stereotypes of ability as a result of using the representa-
, due to selective
tive heuristic that exaggerates empirical reality
Bordalo et al. 2016
)
(
Schwartzstein
attention  that  discounts  how,  for  example,  context  affects  behavior
(
,  or  because  of  coarse  categorization  of  experiences  with  a  particular  group
2014
)
. In our setting, such stereotyping corresponds to distor-
Fryer and Jackson 2008
(
)
 ˆ
 . As also noted in Schwartzstein
tions in the subjective belief about average ability,
   g
  μ
, the discrimination literature has tended to classify discrimination driven by
2014
(
distorted stereotypes as taste-based.8 However, we demonstrate that biased beliefs
lead to patterns of discrimination that substantially differ from those that arise in
taste-based models in which evaluators have animus toward a particular group
i.e.,
(
. This is one reason we clearly distinguish between dis-
preference-based partiality
crimination due to incorrect beliefs and discrimination due to preferences.

)

)

Subjectivity of Judgment: Uncertainty over the assessment criteria, which we refer
to  as  subjectivity  in  judgment,  increases  the  variance  of  potential  evaluations  for  a
given level of an attribute
 and reduces the expected
Olson, Ellis, and Zanna 1983
)
(
. The social psychology literature argues
consensus between evaluators
Kelley 1973
)
(
 and
Fiske et al. 1991
that such subjectivity is “quite vulnerable to stereotypic biases”
)
(
Biernat, Manis, and Nelson 1991; Snyder et al.
increases the scope for discrimination
(
. Indeed, researchers have documented greater reli-
1979; Danilov and Saccardo 2017
)
ance on beliefs about group statistics when judgment is more subjective
see Fiske and
(
. As judgment becomes more objective, the available infor-
Taylor 1991, for review
)
mation provides more precise signals about the underlying attribute. This decreases
the  reliance  on  group  statistics  in  forming  assessments,  and  therefore,  reduces  the
potential for belief-based discrimination. Target groups anticipate greater scope for
discrimination  when  judgment  is  more  subjective  and  in  response,  generate  output
with more objective assessment criteria

We model the level of subjectivity in judgment as the precision of the signal of
 . Factors that increase subjectivity, such as uncertainty over the evalua-
quality,
tion criteria and noisier information sources, decrease the precision of the signal.

 τ η

Parsons et al. 2011
(

.
)

8 For example, Price and Wolfers
(

 suggest that their findings of own-race partiality of basketball referees
)
are not driven by a preference against members of a particular group, but rather by implicit associations between
race and the likelihood of violence. Such discrimination is classified as taste-based, because beliefs about these
Bertrand, Chugh, and Mullainathan 2005; Greenwald, McGhee,
associations influence behavior subconsciously
and Schwartz 1998

2010

(

.

)

THE AMERICAN ECONOMIC REVIEWOCTOBER 20193407

Our  theoretical  results  match  the  empirical  findings  on  subjective  judgment:  we
will  show  that  a  decrease  in  signal  precision  leads  to  greater  reliance  on  beliefs
about group statistics to assess quality, and therefore, greater scope for belief-based
discrimination.

B. Initial Discrimination

We first compare how belief- and preference-based partiality impact initial eval-
uations.  We  show  that  a  comparative  static  on  how  initial  discrimination  varies
with the subjectivity of judgment
 can distinguish
between these two sources.

i.e., the precision of the signal

)

(

 ˆ
   M  )
   μ

Consider the evaluation of the first task from a worker of gender  g  by an eval-
 ˆ
   about  average  ability,  preference
,
uator  who  has  subjective  prior  beliefs
   F
 (  μ
s
c
 .  Given  these  prior  beliefs  about  ability,  the
 ,  and  observes  signal
parameter
 F
 1
 ˆ
  and preci-
evaluator’s prior belief about quality is normally distributed with mean
   g
  μ
q
 , i.e.,
 . The initial signal has conditional
sion
 τ q    ≡   τ a    τ ϵ  / ( τ a   +  τ ϵ  )
 1    ∼
q
q
s
 . Given the prior belief and signal distribution, the
1
,
distribution
 1
 1    ∼
 1   |
 (
/ τ η  )
s
   is  also  nor-
evaluator’s  posterior  belief  about  quality  conditional  on  observing
 1
 ˆ
s
   g   +  τ η
 τ q     μ
, the optimal evaluation
 _  τ q   +  τ η
 (
)

q
s
mally distributed,
 1    ∼
 1   |
is equal to

1 _  τ q   +  τ η    ) .

 ˆ
,
   g
 (  μ

/ τ q  )

  From

 1
,

N

N

N

1

2

(

4

(

)

h
 v
 (

,
 1

s
,
 1

g

 ˆ
s
   g   +  τ η
 τ q     μ
 1
c
  _  τ q   +  τ η
 g  .
  −

)   =

Higher signals and higher expected ability result in higher evaluations: the optimal
 ˆ
s
 .
  and
evaluation is strictly increasing in
   g
 1
  μ
Initial  discrimination  depends  on  the  evaluator’s  preferences  and  prior  beliefs
, initial discrimination is independent of the signal and equal

4

about ability. From
(
to

)

)

(

5

 D

,
 1

h
 (

s
 1  )   =   (

 τ q
 ˆ
 ˆ
c
 _  τ q   +  τ η    )  (  μ
   F  )  +
   M   −   μ
s
h
There  is  initial  discrimination  against  females,  i.e.,   D
0 ,  if  and  only  if
,
 1  )   >
 1
 (
 ˆ
 ˆ
c
0 .
  or
the evaluator has belief-based or preference-based partiality,
 F    >
   M
   F    <    μ
  μ
Therefore, discrimination on the first task stems from an evaluator’s own partiality;
it does not depend on her beliefs about the partiality of other evaluators.

 F  .

It is not possible to identify the source of discrimination from observing initial
evaluations at a single set of parameters. For any level of preference-based partiality,
there exists a level of belief-based partiality that leads to equivalent initial evalua-
tions and discrimination, and vice versa.9 Therefore, we need a richer cross-section
of evaluations to identify the source.

9 For  any  evaluator  with  beliefs
1
1
1
 ˆ
 ˆ
c
   and  preference  parameter
0 ,  an  evaluator  with  preference
  F
    M
    F
  μ
   >    μ
   =
1
2
2
1
2
1
 ˆ
 ˆ
 ˆ
 ˆ
 ˆ
c
   chooses  equivalent  evaluations  and
0   and  beliefs
parameter
    M
    M
    F
 ) / ( τ q   +  τ η  )   >
    M
   =   τ q   (  μ
  F
    F
   =    μ
   =    μ
  μ
  −   μ
. Note that the first evalu-
exhibits an equivalent level of discrimination. This follows immediately from
)
(
ator has belief-based partiality and the second has preference-based partiality.

 and
)

4

5

(

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 10

3408

Our first result shows that varying the level of subjectivity in judgment differ-
entially  impacts  discrimination  depending  on  whether  it  is  due  to  preference-  or
belief-based partiality. This comparative static can be used to identify the source of
discrimination.

Subjectivity of Judgment

PROPOSITION 1
(
tiality, initial discrimination is decreasing in the precision of the signal
erwise, initial discrimination is constant with respect to
perfectly objective,
ator has preference-based partiality.

: If the evaluator has belief-based par-
  and oth-
 . As the signal becomes
 , there is initial discrimination if and only if the evalu-

 τ η    →  ∞

 τ η

 τ η

)

As the signal provides more precise information about quality, the evaluator’s belief
about the worker’s ability has a smaller impact on the evaluation. Therefore, differ-
ences in beliefs about ability, i.e., belief-based partiality, translate into smaller differ-
ences in evaluations and less discrimination. In the limit, when quality is perfectly
observable, differences in beliefs about ability do not lead to discrimination: although
an evaluator with belief-based partiality expects lower quality from female workers ex
ante, male and female workers who generate the same signal receive identical evalu-
ations. In contrast, when the evaluator has preference-based partiality, a more precise
signal of quality does not mitigate the animus toward female workers. Even if quality
is perfectly observable, the female workers will still face discrimination.

This  analysis  extends

neous  beliefs  or  preferences.  Aggregate  discrimination  is  equal  to   D
c
E
 F  ]
=   ( τ q  /( τ q   +  τ η   ))
 π   [
ately follows.

to  a  setting  where  evaluators  have  heteroge-
 1  )
 , and an analogue to Proposition 1 immedi-

 ˆ
 ˆ
E
   F  ]  +
   M   −   μ
 π   [  μ

h
 (

,
 1

s

C. Dynamics of Discrimination

We now focus our attention on belief-based partiality and study how discrimi-
nation evolves across a sequence of tasks. We show that a discrimination reversal
between the initial period and a subsequent period can distinguish between belief-
based partiality with a correct versus misspecified model of inference. Throughout
0
c
this section, we assume that there is no preference-based partiality,
for all evaluators.

c
 M    =
 F    =

Beginning in the second period, evaluations from prior rounds provide infor-
mation about the worker’s ability. A prior evaluation reflects both the prior signal
of  quality  and  the  prior  evaluator’s  belief  about  the  worker’s  ability. Therefore,
interpreting  prior  evaluations  requires  a  model  of  other  evaluators’  beliefs.  We
focus on two cases. In the first, evaluators share a common belief about the dis-
tribution of ability by gender, and this is common knowledge. This case nests the
correctly specified model, in which evaluators also have correct beliefs about the
distribution  of  ability  by  gender.  In  the  second,  evaluators  have  heterogeneous
beliefs: some evaluators have belief-based partiality toward men and believe that
all evaluators share the same beliefs, while other evaluators have no belief-based
partiality but are aware that some evaluators do. Since there is only one correct
distribution of ability for each gender, this heterogeneity implies that at least one
type of evaluator has a misspecified model of inference.

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019

3409

We show that these two cases make different dynamic predictions about the pat-
tern of discrimination. Specifically, we show that a discrimination reversal does not
arise in the first case, which nests the correctly specified model. Therefore, observing
a discrimination reversal suggests that some evaluators have misspecified models of
inference. The second case illustrates one possible misspecified model in which a
reversal can arise.

Impossibility of Reversal in Correctly-Specified Model.—Suppose that all evalu-
ators share a common prior belief about the distribution of ability by gender, have
belief-based  partiality,  and  this  is  common  knowledge:  that  is,  evaluators  have  a
correct  model  of  other  evaluators.  In  our  framework,  this  is  captured  by  a  single
1 .
type
θ
In the first period, a female worker is subjected to stricter standards than a male.
, let

 ˆ
  and a correctly specified type distribution,
   (θ)   =
 π

 ˆ
 ˆ
  with beliefs
   M
   F    <    μ
  μ

Inverting the optimal evaluation from

4
)

(

6

(

)

v,

 ˆ
,
   g
   μ

1

 s

 (

)   ≡   (

 τ q   +  τ η
v
 _  τ η
 )

 −  (

 τ q
 ˆ
 _  τ η    )    μ
   g

1

1

v,

s
 (

)   >

 ˆ
,
   F
   μ

 ˆ
,
   M
   μ

denote  the  signal  required  to  receive  evaluation   v   in  period   1   when  the  evaluator
 ˆ
 . In order to receive the same evaluation as the male worker, the female
has belief
   g
  μ
must  produce  a  higher  signal  of  quality  to  offset  the  lower  belief  about  her  abil-
v,
ity,  s
 . Therefore, a given evaluation is a more positive signal
)
 (
of a female worker’s ability than a male’s. This decreases the difference between
the posterior beliefs about the female and male workers’ average abilities, thereby
reducing  discrimination  in  the  next  period.  However,  despite  the  stronger  signal
from  the  female  worker,  the  higher  prior  belief  about  the  male  worker’s  average
ability still maps into a higher posterior belief, and the beliefs about the male and
female worker do not reverse. Hence, discrimination does not reverse. The analysis
in subsequent periods is analogous: evaluators’ beliefs about the average ability of
male and female workers continue to move closer together following similar evalua-
tion histories, but do not reverse. This brings us to our first dynamic result.

: Suppose there is a single type of eval-
PROPOSITION 2
(
uator with belief-based partiality and no preference-based partiality. Then fixing an
evaluation history, discrimination decreases across periods but never reverses.

Impossibility of Reversal

)

An immediate implication of Proposition 2 is the impossibility of a reversal in the
correctly specified model. Therefore, observing a reversal is indicative of some form
of  misspecification,  either  in  evaluators’  beliefs  about  average  ability  by  gender,
evaluators’ models of other evaluators, or both.

A key feature of social learning settings, such as our model, is the endogenous
informational content of evaluations. In particular, the signal required to receive a
given evaluation is decreasing in the prior belief about average ability, as shown in
. Therefore, the prior belief about average ability impacts the posterior distribu-
6
(
)
tion of ability through two channels, which move in opposite directions:
 the prior
(
distribution of ability directly enters the Bayesian update, and this distribution has
 the distribution of the
an increasing monotone likelihood ratio in its mean; and
)

ii

)

(

i

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 10

3410

signal that yields a given evaluation has a decreasing monotone likelihood ratio in
the prior belief about average ability. The proof of Proposition 2 lies in establish-
ing  that  the  first  effect  dominates.  Therefore,  the  posterior  mean  is  increasing  in
the prior mean, so if evaluators believe that males have a higher prior mean than
females, then following a given signal, they also believe that males have a higher
posterior mean.10

i

 the existence of a type with belief-based partiality

Possibility  of  Reversal  in  Misspecified  Model.—Next,  we  present  one  form  of
misspecification that leads to a discrimination reversal. The key features of the setup
that drive the reversal are
to
  the  existence  of  a  type  that  believes  that
  and
generate  initial  discrimination
there exists another type with more extreme belief-based partiality
to generate the
reversal
. This is a possibility result, in the sense that it demonstrates one possible
)
way to generate a reversal. Other forms of misspecification can also lead to rever-
sals.  Theoretically  or  empirically  distinguishing  between  different  forms  of  mis-
specification is beyond the scope of this paper.

ii

(

(

(

)

(

)

)

(

 θ 1

Suppose there are two types of evaluators. The first type

Pronin, Lin, and Ross 2002
. With probability  p

  uses a heuristic to
form beliefs about the relationship between ability and gender, which leads to belief-
1
1
 ˆ
 ˆ
 . This type is not aware of its bias, and
based partiality that favors men,
    M
    F
   <    μ
  μ
 ˆ
1 , such as in the case
believes that other evaluators have the same beliefs,
   1   ( θ 1  )   =
  π
Ross,
 or false consensus effect
of the bias blind spot
(
)
 . We
 , an evaluator is type
1
0,
Greene, and House 1977
 θ 1
)
  ∈   (
refer to this type as the heuristic type. The second type
  has no belief-based par-
2
2
 ˆ
 ˆ
 , but is aware that some evaluators do; it has a correctly specified
tiality,
    M
    F
   =    μ
  μ
 ˆ
p . We refer to this type as the impartial
model of the type distribution,
   2   ( θ 1  )   =
  π
type. To close the model, assume that both types have the same belief about the aver-
2
1
 ˆ
 ˆ
  denote this belief. Importantly,
age ability of male workers,
    M
    M
   =    μ
  μ
this heterogeneity in the subjective belief about the average ability of female work-
ers implies that at least one type has incorrect beliefs.11

 ˆ
 , and let
   M
  μ

 θ 2

)

In the first round, a heuristic evaluator discriminates against females, while an
impartial evaluator exhibits no discrimination. Aggregate initial discrimination is a
weighted average of these two type’s evaluations,

7

(

)

 D

h
 (

,
 1

s
 1  )   =

p

 τ q
1
 ˆ
 ˆ
 _  τ q   +  τ η    )  (  μ
    F
   M   −   μ
 )   >
 (

0

.

10 If the informational content of evaluations did not depend on the prior distribution of ability—for example,
if  evaluators  simply  reported  the  observed  signal   s —then  the  property  that  beliefs  do  not  reverse  would  follow
immediately. This is because the monotone likelihood ratio property
 is preserved under Bayesian updating
(
with respect to a fixed signal distribution.

MLRP

Bordalo et al. 2016

11 The literature on heuristics and biases provides a foundation for such a model. Type

  can capture evaluators
who use a “representativeness” heuristic to form beliefs about the population distribution of ability, i.e., stereotyp-
ing
  can capture evaluators who have accurate
(
beliefs about the population distribution of ability by gender and are aware that a subset of evaluators stereotype. In
online Appendix D, we use observational data to provide a foundation for type
  in our experimental setting. We
show that using the “representativeness” heuristic will magnify small performance differences in the observational
data, leading to belief-based partiality with bias.

 and are not aware of their cognitive bias. Type
)

 θ 1

 θ 1

 θ 2

)

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019

3411

i
 ˆ
v
v
  denote an evaluator of type
Following evaluation
 , let
    F
 1  )
 1
  (
  μ
 ˆ
v
about the average ability of a female worker and
   M   (
 1  )
  μ
about the average ability of a male worker

 ’s posterior belief
  denote the posterior belief

 θ i

which is the same for both types

.

)

(
A  heuristic  evaluator’s  beliefs  about  ability  evolve  in  the  same  manner  as  the
beliefs of an evaluator in the single-type model, since the heuristic type believes that
all evaluators have the same beliefs. From Proposition 2, the heuristic type’s beliefs
1
 ˆ
 ˆ
v
v
 , and therefore, the type continues to discriminate
do not reverse,
   M   (
    F
 1  )
 1  )   <    μ
  (
  μ
against  females  in  the  second  period.  In  contrast,  an  impartial  evaluator  is  aware
that  with  positive  probability,  a  female  worker  was  evaluated  by  a  heuristic  type
and faced discrimination in the first period. Therefore, the impartial type’s poste-
2
 ˆ
 ˆ
v
v
 , and
rior belief about average ability immediately favors females,
   M   (
    F
 1  )
 1  )   >    μ
  (
  μ
this  type  discriminates  against  males  in  the  second  period. As  in  the  first  period,
aggregate discrimination in the second period is a weighted average of these two
type’s evaluations. Whether an aggregate discrimination reversal occurs depends on
whether the impartial type’s posterior belief favors females enough that it reverses
the aggregate posterior belief about average quality. Proposition 3 establishes that
indeed, given any initial evaluation or any second period signal, aggregate discrim-
ination reversals are possible.

 θ 1

PROPOSITION  3
type

(

Possibility  of  Reversal
0,

1

)

:  Suppose  evaluators  are  the  heuristic
p .

  ∈   (

  with probability  p

  and the impartial type
)
 , there exist cutoffs   p –
  such
s
  and
v
  For any initial evaluation
1
0,
  ¯
 1
   ∈  ℝ
)
  ∈   (
p –
   and a high enough
0,
)
s –  , aggregate discrimination reverses in the sec-

that for a low enough share of heuristic types  p
second period signal,
s
s
ond period,  D
 2  )   <

  with probability  1

 2    >
0 .

  ∈   (

 θ 2

 −

i
)

(

v
,
 1
 (
s
  For any second period signal
)

ii

  (

  and   v –
 , there exist cutoffs   p –
1
0,
 2
)
  ∈  ℝ
p –
    and  a  low
such  that  for  a  low  enough  share  of  heuristic  types   p
0,
′)
v –  , aggregate discrimination reverses in the
enough initial evaluation,
v
 1    <
0 .
s
second period,  D
 2  )   <

′  ∈   (
  ∈   (

v
,
 1
 (

Increasing  the  prevalence  of  heuristic  evaluators  impacts  second  period  dis-
crimination through two channels. First, it increases the difference in the impartial
type’s second period beliefs about the average ability of a male and a female. This
is because a larger share of heuristic evaluators means that it is more likely that the
female faced initial discrimination and received the higher signal required to receive
a given evaluation from the heuristic type, rather than the lower signal required to
receive this evaluation from the impartial type. Second, it increases the probability
that  the  second  period  evaluator  is  a  heuristic  type.  Since  the  heuristic  type  still
discriminates against females in the second period, it is more likely that a female
will continue to face discrimination. The first effect dominates for low  p , while the
latter effect dominates for high  p . This leads to a non-monotonicity in how second
period discrimination changes with respect to  p . Further, discrimination is always
zero at  p
0 , as all evaluators are impartial, and discrimination is always positive
  =
at  p
1 , as this corresponds to a single type of evaluator with belief-based partial-
ity. Figure 1 illustrates the possibility of a reversal.

  =

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 10

3412

)

2
s

,
1
v

(

D

0.2

0.15

0.1

0.05

0

0.05

−

0.1

−

0.15

−

0.2

−

Discrimination against males

Discrimination
against females

0

0.1

0.2

0.3

0.4

0.5

0.6

0.7

0.8

0.9

1

p

Figure 1. Second Period Discrimination, as a Function of the Proportion of Heuristic Evaluators

Proposition  3  does  not  rely  on  the  assumption  that  the  impartial  evaluators
exactly understand the bias of the heuristic evaluators or accurately estimate their
prevalence in the population. It is straightforward to derive a similar result when the
impartial evaluators under- or overestimate either the level of the bias of heuristic
evaluators, their frequency, or both.

D. Discussion of Results

i

(

)

)

(

ii

In summary, our theoretical results show that

 it is not possible to identify
the source of discrimination from a single round of evaluations with a fixed level
  varying  the  subjectivity  of  judgment  can  identify  whether
of  subjectivity;
the source of discrimination is preference-based or belief-based;
 a reversal
of  discrimination  is  not  possible  in  a  correctly-specified  model  of  belief-based
partiality,  and  therefore  points  to  belief-based  partiality  with  misspecification.
Before moving to the empirical section, we briefly discuss the robustness of our
theoretical  framework  to  other  specifications  and  relate  it  to  several  alternative
 models.

iii

(

)

Robustness

Alternative Distributions of Ability: We combine a partial analytical derivation
with numerical analysis to illustrate that the impossibility of a reversal in the correctly
 is robust to other distributions of ability, including
specified model
the beta distribution, exponential distribution, gamma distribution and a setting with

Proposition 2

(

)

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019
3413

see online Appendix A

.12 The key feature that drives the
binary ability and quality
)
(
impossibility of a reversal is that the ability distribution satisfies the monotone like-
lihood ratio property
 with respect to the parameter that varies by gender.
MLRP
)
 and
The MLRP is commonly assumed in information economics
holds for many other families of distributions. Propositions 1 and 3 are also robust to
alternative distributional assumptions. It is straightforward to extend Proposition 1
analytically. By similar intuition to Proposition 3, it is possible to generate reversals
in misspecified models with other ability distributions.

Milgrom 1981

)

(

(

Coarse Evaluations: We assume that the space of possible evaluations is iso-
morphic to the space of beliefs about expected quality. In reality, the space of pos-
sible evaluations may be coarser than the evaluator’s belief about expected quality.
For example, the evaluator may only be able to accept or reject a task, or rate it on
a scale of 1 to 5. When this is the case, it will not be possible to perfectly infer the
signal an evaluator observed from the reported evaluation and information will be
lost. In online Appendix B.1, we show that an analogue of Proposition 2 holds for
coarse evaluations. In particular, a discrimination reversal does not occur between
the first and second period when evaluators have common knowledge of the same
beliefs about the distribution of ability for men and women.

Shifting Standards: Another relevant feature for our setting is how the standard
of evaluation may change with respect to reputation. Higher reputation often leads
to increased responsibilities and privileges, which require greater ability to manage
effectively. As such, individuals may be subject to increasingly higher benchmarks
as their level of seniority increases to avoid erroneously granting responsibility to
someone who is unprepared. Our framework can easily be adapted to capture shift-
 with respect to reputation. We say
ing standards
a worker faces shifting standards if, conditional on receiving a positive initial eval-
uation, the worker faces a stricter standard in the second period: a higher signal is
required to receive a given evaluation, relative to the signal required for the same
evaluation in the first period. We explore this extension in online Appendix B.2.

Biernat, Vescio, and Manis 1998
(

)

Alternative Models

Attrition:  Suppose  that  workers  exit  the  worker  pool  with  positive  probability
after completing each task, and lower ability workers exit at a higher rate than higher
ability workers. In this case, the content and the length of the worker’s evaluation
history provide information about ability. If male workers exit at a lower rate than
female workers, conditional on sharing similar evaluation histories, then the length
of  the  evaluation  history  has  different  informational  content  for  male  and  female
workers. If evaluators’ subjective prior beliefs about ability favor males, then this
differential attrition will shrink these initial differences. It can even lead to a  reversal

12 Analytical results are possible for the normal distribution, as a normal ability distribution is the conjugate
prior for a normal signal distribution. This means that the posterior distribution of ability is also normally distrib-
uted, which allows for a recursive representation of the belief-updating process and a closed-form characterization
of the evolution of beliefs. When the conjugate prior property does not hold, as is the case for the other distributions
we consider, a combination of analytical and numerical analysis is necessary.

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 103414

when low-ability women exit at a fast enough rate that distributions following lon-
ger histories favor women. In contrast to Proposition 3, such a reversal can occur
even when all evaluators have correctly specified models.

In  Section  IID  we  empirically  test  for  differential  attrition  by  gender.  We  use
observational data from the forum to show that males and females with similar eval-
uation histories leave the market at similar rates. Therefore, there is no evidence for
differential attrition in our experimental setting. Evaluators may incorrectly believe
that attrition differs by gender, but in this case, they have a misspecified model.

Differential  attrition  may  drive  discrimination  reversals  in  other  labor  market
settings. It is therefore important to empirically measure attrition in order to rule
out differential attrition as a potential driver of the reversal. Our empirical analysis
demonstrates how one could measure attrition based on observable data from the
setting of interest and test whether it differs by gender.

Gender Differences in Variance of Ability: If the variance of ability differs for
females and males, then discrimination may be non-monotonic in the signal of qual-
ity. It is straightforward to show that this can lead to a discrimination reversal when
the  signal  of  quality  is  imprecise.  Regardless  of  the  precision  of  the  signal,  this
model predicts higher variance in the evaluations of the group that has higher vari-
ance in ability, relative to the group that has lower variance in ability. In Section
IID  we  empirically  test  for  differences  in  the  variance  of  evaluations  by  gender.
We  use  observational  data  from  the  forum  to  show  that  the  evaluations  of  males
and females have similar variances for tasks with precise signals. Therefore, in our
experimental  setting,  we  find  no  evidence  for  gender  differences  in  the  variance
of  ability.  Differential  variance  may  drive  discrimination  reversals  in  other  labor
market settings. Our empirical analysis demonstrates how one could use variance
in evaluations, which is based on observable data, to proxy for variance in ability,
which is unobservable, and test whether it differs by gender.

Heterogeneous  Preference-Based  Partiality:  Suppose  that  all  evaluators  have
correct beliefs about the ability distributions for male and female workers, but vary
in their preference-based partiality against females. In this setting, there is no dis-
tribution over types that can simultaneously capture the following two predictions:
0 , and
i
 initial discrimination against females when judgment is subjective,
 τ η    >
)
(
0 .
 no initial discrimination against females when judgment is objective,
ii
(
)
  has preference param-
To see this, consider a type space
c
,  when  there  are
5
 .  From
eter
   =   μ M
)
(
i
c
E
s
h
multiple  types,  initial  discrimination  is  equal  to   D
 .  Prediction
,
 ]
 π   [
  F
 1  )   =
 1
 (
c
E
 .  Therefore,  when
  requires
i
 π   [
 τ η
(
)
i
c
E
0 ,  there  will  also  be  discrimination  when  judgment  is  objective  and
 ]   >
 π   [
  F
  is  not  possible.  Given  this,  simultaneously  observing  evidence  for
ii
prediction
)
(
 rules out discrimination that is caused by preference-based
 and
i
predictions
)
(
partiality with heterogeneous preference parameters. In Section IIC, we demonstrate
how to empirically test these two predictions in our experimental setting.

Θ
i
i
 ˆ
   and  correct  beliefs,
   =   μ F
    F
  F
  μ

  where each type
i
 ˆ
   and
    M
  μ

   is  independent  of

i
 ]   >
  F

0 .  But   D

 θ i    ∈  Θ

s
 1  )

 τ η    ≈

h
 (

,
 1

ii

(

)

Self-Fulfilling  Beliefs:  As  discussed  in  Section  IA,  self-fulfilling  beliefs
  explores  how

are  another  form  of  belief-based  discrimination.  Fryer

2007

(

)

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019

3415

 discrimination dynamically evolves when it is driven by self-fulfilling beliefs. He
shows that discrimination can reverse in the second period if there exist equilibria
in which one group coordinates on an equilibrium with higher initial standards and
looser second period standards, while the other group coordinates on looser initial
standards and more stringent second period standards.13 Thus, in Fryer
, the
reversal depends on how coordination dynamically evolves, while in our model, the
reversal stems from the endogenous informational content of prior evaluations. In
Fryer’s setting, multiple equilibria always exist: there are also equilibria in which
either group faces discrimination in both periods and equilibria in which all work-
ers are treated equally. Therefore, almost all outcomes are possible, conditional on
observables.

2007

(

)

II.  A Field Experiment

We conduct a field experiment on an online Q&A mathematics forum. The forum
is part of a family of forums where, in 2017 alone, 3,517,799 questions were asked
and  4,299,077 answers were  provided. With over 10 million registered users, the
forums are an important resource for students and researchers in STEM. We exam-
ine gender discrimination by posting content to the forum in the form of questions
and answers.14 In addition to the experiment, we exploit two additional data sources
to explore the predictions of the theoretical framework. First, we collect observa-
tional data from the forum to further study potential mechanisms, including estimat-
ing distributions from publicly available statistics. Second, we use a private dataset
provided by the forum on the voting behavior of users to run additional robustness
tests.

A. Description of Forum

tasks

Organizing terms with respect to the theoretical framework, users
(

 gen-
, the quality of which are then assessed by
erate content in the form of posts
. There are two main types of tasks: questions
other users on the forum
and answers
. See online Appendix C.1 for
)
examples of both types of posts. Users can choose to evaluate either type of post
by assigning an upvote or downvote to it. Voting is anonymous: other users cannot
observe any information about the identity of the user who cast a vote.15

in response to other users’ questions

evaluators

workers

)

(

)

)

(

(

The forum offers written guidelines for evaluating posts, and these guidelines are
actively discussed on the forum’s message boards. Voting is meant to serve a dual
 upvoting is meant to highlight a quality post while downvoting is meant
purpose:
(
 upvoting rewards the user for a high  quality
to discourage low quality posts, and
(

i
)

ii

)

13 The existence of an equilibrium in which beliefs flip requires fairly strict conditions. In relation to our set-
ting, the payoff to an evaluator for accurately evaluating a product must be substantially higher than the payoff to
the worker for receiving a positive evaluation. This assumption is likely not satisfied in many settings of interest,
including the experimental setting we consider in Section II and settings with competition.
14 The experiment was pre-registered in the AEA RCT Registry, AEARCTR-0000950.
15 The  anonymous  setting  ensured  that  the  decisions  of  users  interacting  with  our  posts  were  not  subject  to

experimenter demand effects.

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 103416

post while downvoting punishes him or her for a low-quality post.16 The second point
stems  from  the  fact  that  users  earn  publicly  observable  reputation  points  from  the
votes they receive for their posts. An upvote earns 5 reputation points on questions
and 10 reputation points on answers, while a downvote deducts 2 reputation points for
both questions and answers.17 Reputation unlocks privileges, such as the ability to edit
and comment on others’ posts or tag questions as duplicates. It can also be used as a
currency through the assignment of “bounties”: users can spend their reputation points
to post a question with a bounty that will be awarded to the highest quality answer, as
determined by the question poster, to increase the quality of answers.

)

(

(

upvotes  minus  downvotes

a signal
population  beliefs

The theoretical setup in Section I maps onto the key features of the experimental
environment. Each post on the forum  is  accompanied by clearly visible informa-
tion summarizing its evaluation by the community—the associated net number of
votes
—and  information  about  the  poster—his  or  her
username and current reputation. In judging the quality of a post, the evaluator can
, as well as draw inference from the gender
read the content of the post
)
of  the  username
. The
  and  the  reputation
number of reputation points serves as a summary statistic of past quality—greater
reputation corresponds to the evaluators observing a higher sequence of signals on
prior posts—while clicking on the user’s profile reveals the full history of upvotes
and downvotes by post. The informational content of reputation and prior evalua-
tions  endogenously  depends  on  the  voting  behavior  of  other  users  on  the  forum.
Therefore, interpreting these evaluations requires a model of how past voting behav-
ior depends on the prior evaluators’ beliefs and preferences. For example, an evalua-
tor who is aware that female users face more exacting initial standards may take this
into account when assessing a question from a high-reputation female.

evaluation  history

(

)

)

(

Additionally,  higher  reputations  earn  users  greater  privileges  on  the  forum.
Reputation  allows  users  to  advance  through  the  ranks,  with  each  rank  correspond-
ing to a new set of privileges. This includes privileges to “supervise” other users: for
example, to edit, comment on, flag, downvote and close other users’ posts. In turn, the
evaluation process mirrors promotion decisions in labor market contexts: the higher a
user’s reputation, the more influence he or she has over other users on the forum.

B. Experimental Design

The ability to exogenously vary the gender and reputation associated with a user
makes this an ideal setting for testing the dynamic predictions of different sources of
discrimination. Comparing evaluations of question and answer posts allow us to test
the predictions of how discrimination varies with the level of subjectivity in judgment.

Posting Questions.—We generated a series of original mathematics questions and
posted them under male and female usernames on accounts with low and high rep-
utations. We opened 280 new accounts, with 140 male usernames and 140 female

16 While we use votes as our primary criterion of differential evaluation, discrimination can also manifest in less
Bohren, Imas,
, we use natural language processing to document systematic differences in the ways in which

objectively measurable ways, such as the language used in response to a post. In a companion paper
(
and Rosenberg 2018
users respond to male versus female posters.

)

17 It is not possible for a user’s reputation to fall below 1.

THE AMERICAN ECONOMIC REVIEWOCTOBER 20193417

  =

(

70 male and 70 female

usernames.18 Each account was associated with its own email address, username,
and password. Of these accounts, 140
70 with female usernames and 70 with male
(
usernames
 were left as new accounts; these comprised the Novice accounts. For
)
, we manually built up the reputa-
the other 140 accounts
tion to the top twenty-fifth percentile of reputation on the forum; at the time of the
experiment, this corresponded to a reputation of at least 100. Research assistants
earned  reputation  on  each  account  by  posting  content  until  the  accumulated  rep-
utation reached 100. Once an account reached at least 100, the research assistant
stopped posting content. Because reputation was accumulated through the actions
 of other users on the forum, we could not control the exact number of rep-
votes
(
utation points associated with each account: the mean reputation on these accounts
was  M

155.23 . These accounts comprised the Advanced accounts.

)

)

Critically, upon achieving a high reputation, we re-randomized the gender of the
username  on  the Advanced  accounts:  35  accounts  that  were  built  up  under  male
usernames were switched to female, and 35 female accounts were switched to male;
the remaining 70 accounts received a new username of the same gender. Importantly,
when  a username is switched, all past and future activity on the account became
associated with the new username. That is, all previous posts now reflect the new
username, and no public record of the name change is available. Re-randomizing
the gender of the usernames avoids issues of endogeneity associated with, for exam-
ple, female accounts requiring different quality posts to achieve the same level of
reputation as male accounts. After reassigning usernames, the new female and male
 M
154.57 , respec-
accounts had similar reputation levels
(
tively,  p

155.89  versus  M

  =

  =

.

Our goal was to write high-quality questions that would be well received on the
forum. Content on the forum ranges from high school arithmetic to upper-level grad-
uate mathematics. Questions are tagged by topic, e.g., real analysis, combinatorics.
Users are discouraged from posting questions directly from textbooks or duplicating
content that is already posted; such posts are flagged and routinely closed by mod-
erators. In order to minimize the chance that our content was flagged, we wrote 280
novel mathematics questions ranging in level of difficulty from upper-level under-
graduate to early graduate. These questions were randomly assigned to one of the
four conditions: male novice, female novice, male advanced, or female advanced.

0.82
)

  =

We  posted  questions  on  a  predetermined  schedule  to  avoid  altering  the  usual
activity  on  the  forum,  i.e.,  flooding  the  forum  with  content.  Research  assistants
posted  one  question  at  least  20  minutes  apart  between  5  pm  and  10  pm,  Monday
through Thursday. Data on the community response to the questions, e.g., upvotes,
downvotes,  number  of  answers,  were  collected  seven  days  after  posting  for  each
question, both in numerical form and as screenshots. A total of 7 of the 280 ques-
tions were dropped from our analysis due to forum moderators prematurely closing
the questions before the end of the seven-day window or due to errors in the posting
of the questions

i.e., two questions posted to the same account

.

We measure discrimination as either the average change in reputation points per
.

 or the average number of upvotes net of downvotes per post
(

Net Votes

 Rep

Δ

post
(

)

)

)

(

18 Names were taken from the “Top Names of the 2000s” list created by the Social Security Administration,

https://www.ssa.gov/oact/babynames/decades/names2000s.html.

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 10
3418

The dynamic pattern of discrimination provides a test of the theoretical predictions
outlined in Section I. Conditional on observing discrimination between male and
female Novice accounts, a mitigation in its intensity for Advanced accounts is con-
sistent with belief-based partiality, including the case of statistical discrimination
where beliefs are correct, while a reversal of discrimination for Advanced accounts
is evidence for biased belief-based partiality.

)

We  do  not  make  a  prediction  on  how  evaluations  vary  by  reputation  within  a
given gender or pooled across genders, due to the potential for shifting standards
.  Higher  reputation  is  indicative  of  higher  ability,  which  leads  to  a
Section  ID
(
higher assessment of quality on a given post. But as previously discussed, reputa-
tion serves both the purpose of highlighting a quality post and rewarding the poster.
Therefore, posts by high reputation users may be held to higher standards of quality,
since reputation determines which users rise through the rungs to become modera-
tors and receive other privileges. For example, a novice user may be rewarded with
an upvote for a low-level calculus question, but an advanced user may not be. In our
experiment, randomization ensures that the average quality of questions posted to
novice accounts is approximately the same as that of questions posted to advanced
accounts. Since the two effects point in opposite directions, the overall directional
prediction regarding the effect of reputation on upvotes per question is ambiguous.

Posting  Answers.—We  generated  original  answers  to  mathematics  questions
posted by other users on the forum, and posted them under male and female user-
names.  To  examine  how  the  subjectivity  of  judgment  affects  discrimination,  we
compared  the  evaluations  of  these  answers  to  the  evaluations  of  questions.  The
guidelines for determining whether a post merits an upvote or downvote are differ-
ent for questions and answers. The standard of quality for answers is clear: deter-
mine whether or not the answer is correct. In contrast, there are multiple standards
for judging the quality of a question, including whether it is interesting, novel, or
important for the accumulation of knowledge on the forum. According to our defi-
nition of subjectivity outlined in Section I, this difference in standards of quality
should make judgment of questions more subjective than judgment of answers.

The difference in subjectivity is echoed in the meta-forums for the site. A popular
post asks why the site’s users upvote questions. The poster writes that for answers:
“it’s easy to determine what to upvote. Is it correct?” For questions, this objective cri-
teria does not apply. What criteria do others use? This post has dozens of responses,
including: is the question well-written, non-trivial or insightful, am I curious about
the same question, has the poster made me curious about what they are asking, do
I think it is important and should be visible to others, does it show research effort,
the combination of topic with the reputation of the poster. One response highlights
potential issues with the subjectivity in judgment for questions, noting that voting
on questions may be affected by disliking the topic in general or viewing it as unim-
portant

this response had one of the highest number of upvotes on the forum.
(
To post answers, we created a second set of 140 Novice accounts with no prior
posts,  split  between  70  male  usernames  and  70  female  usernames. We  needed  to
post answers in real time, as questions on the forum are answered fairly quickly and
late answers generally receive little attention. To do so, research assistants worked in
pairs. One member of the pair, the “answerer,” would find a newly posted question

)

THE AMERICAN ECONOMIC REVIEWOCTOBER 20193419

that had not been answered yet and write an answer for it. The “answerer” would
then send the answer and a link to the question to the other research assistant, the
“poster,” who would assign the answer to one of our accounts and post it. The order
of accounts that the answer would be posted to was predetermined: known to the
“poster” but not the “answerer.” As such, the research assistant writing the answer
did  not  know  the  gender  of  the  account  that  the  answer  would  be  posted  to,  and
therefore,  could  not  be  subconsciously  influenced  by  whether  the  answer  would
be posted to a male or female account. As with the questions, answers were posted
between 5 pm and 10 pm, Monday through Thursday. Data were collected seven days
after posting the answer, both in numerical form and as a screenshot. A total of 5 of
the 140 answers were dropped due to errors, e.g., the question was closed before the
seven-day window concluded.

The  theory  in  Section  I  predicts  that  subjectivity  in  judgment,  modeled  as  the
precision of the signal of quality, will affect discrimination differentially depending
on its source. Conditional on observing discrimination on questions, which involve
more subjectivity in judgment, a mitigation of discrimination on answers is indica-
tive of belief-based partiality. In contrast, a similar level of discrimination for both
questions and answers suggests preference-based partiality.

Site Activity.—We continuously scraped the forum for activity to capture relevant
metrics for the experiment and ensure that activity on the forum remained relatively
similar for the duration of the experiment. The turnover in unique active users was
high:  the  average  daily  turnover  was  85  percent  and  the  weekly  turnover  was  92
percent.

C. Experimental Results

We first present results comparing the evaluations of answers versus questions
by gender. Examining how subjectivity of judgment affects discrimination in our
setting enables us to distinguish between preference and belief-based partiality. We
then present results comparing the evaluations of novice versus advanced questions
by gender. This allows us to study the dynamics of discrimination and helps to dis-
tinguish between biased and unbiased belief-based partiality.

. Column 1 of Table 1 shows that regressing

Subjectivity of Judgment.—We first examine the change in reputation
(

 for
)
i.e., the reputation points earned
answers posted to male versus female accounts
on the post
 Rep per answer on gen-
)
der  reveals  no  significant  difference  in  the  evaluation  of  answers  at  conventional
levels. This  result  is  illustrated  in  panel A  of  Figure  2,  which  shows  the  average
 Rep  by  gender.
Δ
Column 2 of Table 1 repeats the analysis using net votes per post as the dependent
variable.19  Together,  these  results  suggest  that  there  is  little  evidence  for  gender
discrimination on answers.

 Rep  by  gender,  and  panel  B,  which  plots  the  distributions  of

 Rep

Δ

Δ

Δ

(

19 Downvotes were very rare in our sample. We obtain similar results when we use only upvotes as the depen-

dent variable

(

online Appendix C.2

.

)

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 10

3420

Table 1—Subjectivity: Effect of Gender on Evaluation of Novice Answers and Questions

Answers only

Questions only

Answers and
questions

Male

Question

Male

×

 question

Constant

Observations

 Rep
1

Δ
(
)
1.38
0.97

−
 (

)

Net votes
2

(
)
0.31
0.17

−
 (

)

Rep
Δ
3
(
)
 2.86
1.32

 (

)

Net votes
4

(
)
 0.58
0.27

 (

)

 4.60
0.69

 (
135

)

 0.79
0.12

 (
135

)

 4.68
0.93

)

 (

135

 0.88
0.19

)

 (

135

−
 (

 Rep
5

Δ
(
)
1.38
1.16
)
 0.08
1.16
)
 4.24
1.64
)
 4.60
0.82

 (

 (

)

 (
270

Net votes
6

−
 (

(
)
0.31
0.22
)
 0.09
0.22
)
 0.89
0.32
)
 0.79
0.16

)

 (

 (

 (

270

Notes: Standard errors from OLS regressions reported in parentheses; Male
Question
1 if question post, 0 if answer; Novice accounts only.

=

1 if male username, 0 otherwise;

=

Panel A. Average

∆

Rep

Panel B. Distribution of

Rep

cdf
)

(

∆

n
o
i
t
a
t
u
p
e
r
n

i

e
g
n
a
h
C

10
9

8
7

6
5

4
3

2

1
0

Female

Male

1

0.8

0.6

0.4

0.2

0

Male

Female

Note: Winsorized at 90 percent

0

5

10

15

20

Figure 2. Change in Reputation for Answers

Δ

Looking at the evaluation of questions posted to novice accounts reveals a sub-
stantially different pattern. We find significant initial discrimination against females:
regressing
 Rep or net votes per question on the gender of the poster reveals that
questions  posted  to  accounts  with  female  usernames  accumulated  significantly
  and  received  significantly  fewer  net
fewer  reputation  points
Table  1,  column  3
(
votes
 than questions posted to accounts with male usernames.
Table 1, column 4
)
These  differences  correspond  to  roughly  0.4  standard  deviations  of  the  average
change in reputation and average number of votes. This result is illustrated in panel
 Rep by gender, and panel A of Figure 4,
A of Figure 3, which shows the average
which plots the distributions of
 Rep by gender. Together, these results suggest that
there is significant evidence for gender discrimination on questions.

Δ

Δ

)

(

Next,  we  directly  compare  responses  to  answer  versus  question  posts  by  gen-
der.  We  first  test  the  difference  in  the  estimated  coefficients  of  the  male  gen-
der  dummy  between  the  question  and  answer  regressions  and  find  that  this

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019

Panel A. Novice accounts

Panel B. Advanced accounts

3421

10
9
8
7

6
5
4
3
2
1
0

n
o
i
t
a
t
u
p
e
r

n

i

e
g
n
a
h
C

10
9
8
7

6
5
4
3
2
1
0

n
o
i
t
a
t
u
p
e
r

n

i

e
g
n
a
h
C

Female

Male

Female

Male

Figure 3. Average Change in Reputation for Questions

Panel A. Novice accounts

Panel B. Advanced accounts

1

0.8

0.6

0.4

0.2

0

0

5

1

0.8

0.6

0.4

0.2

0

Male

Female

Note: Winsorized at 90 percent

Male

Female

Note: Winsorized at 90 percent

10

15
Change in reputation

20

25

30

0

5

10

15
Change in reputation

20

25

30

Figure 4. Distribution of Change in Reputation for Questions

CDF
)
(

2
 χ

(

  (

  (

1

1

Δ

  =

  =

 Rep

)   =

7.87 ;  p

0.01
)

difference is significant for both

6.70 ;  p
 and net votes
)   =
2
. We then present regression results for question and
0.005
)
(
 χ
 Rep and net votes on dummies
answer posts within the same model. We regress
 and the interaction of
corresponding to gender, type of post
gender and type of post
. There is a significant mitigation
(
of  discrimination  against  female  accounts  for  answers,  relative  to  questions:  the
interaction effect between gender and type of post is positive and significant in both
specifications. This implies that the male advantage is significantly larger for ques-
tions, compared to answers.

Δ
question or answer

Table 1, columns 5 and 6

)

)

(

Taken together, these results are inconsistent with discrimination due to prefer-
ence-based partiality. Rather, they support the theoretical prediction on how subjec-
tivity affects discrimination when evaluators have belief-based partiality.

Dynamics of Discrimination.—Next, we examine the dynamics of discrimination
by comparing discrimination toward novice and advanced users. As shown in panel
B  of  Figure  3,  questions  posted  to  advanced  female  accounts  accumulated  more

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 10

3422

Table 2—Dynamics: Effect of Gender on Evaluation Questions, Novice and Advanced

Male

Advanced

Male

×

 advanced

Constant

Observations

Advanced

 Rep

Net votes

Novice and advanced
Net votes

 Rep

Binary

Δ

1

(
)
3.16
1.37

)

−
 (

2

(
)
0.62
0.28

)

−
 (

 7.01
0.97

)

 (

138

 1.38
0.20

 (
138

)

Δ

3

(
)
 2.86
1.36
)
 2.33
1.35

)
6.02
1.91
)
 4.68
0.96

)

 (

 (

−
 (

 (
273

4

(
)
 0.58
0.27
)
 0.49
0.27

)
1.20
0.38
)
 0.88
0.19

)

 (

 (
−
 (

 (

273

5

(
)
 0.17
0.08
)
 0.09
0.08

)
0.40
0.11
)
 0.56
0.06

)

 (

 (

−
 (

 (
273

Notes: Standard errors from OLS regressions reported in parentheses; Male
Advanced

1 if Advanced account, 0 otherwise.

=

1 if male username, 0 otherwise;

=

Δ

 Rep, than those posted to advanced male accounts. This con-
reputation points,
trasts with questions posted on novice female accounts, which accumulated fewer
reputation points than those posted to novice male accounts
. In
)
(
other words, we observe a dynamic reversal of discrimination between novice and
advanced accounts: questions from male users are favored at low reputations, while
questions from female users are favored at high reputations. Figure 4 illustrates this
 Rep on
reversal in the distributions of
questions posted to novice accounts, while panel B shows the distribution of
 Rep
for advanced accounts.

panel A shows the distribution of

panel A of Figure 3

 Rep:

Δ

Δ

Δ

Δ

For advanced accounts, regressing

 Rep or net votes per question on the gen-
der  of  the  poster  reveals  that  questions  posted  to  female  accounts  accumulated
significantly  more  reputation  points  and  net  votes  than  questions  posted  to  male
.  These  differences  in  evalua-
accounts
Table  2,  columns  1  and  2,  respectively
tion  correspond  to  roughly  0.6  standard  deviations  for  both
 Rep  and  net  votes.
This contrasts with the significantly lower evaluation of questions posted to novice
female accounts relative to novice male accounts, as reported in Table 1. Testing
the  difference  in  the  estimated  coefficients  of  the  male  gender  dummy  between
the  Novice  and  Advanced  regressions  reveals  a  significant  difference  for  both

Δ

)

(

2
  (
 χ

2
  (
 χ
(

.

(

1

1

Δ

  =

  =

)   =

)   =

9.88 ;  p

10.05 ;  p

0.002
)

0.002
)

 and net votes
 Rep
Columns 3 and 4 of Table 2 present regression results for Novice and Advanced
 Rep on dummies cor-
accounts within the same model. In column 3, we regress
novice
responding  to  the  gender  of  the  poster,  the  reputation  level  of  the  poster
or advanced
, and their interaction. The interaction between gender and reputation
level is negative and significant, confirming the reversal of discrimination between
the Novice and Advanced accounts. The same pattern of results holds for the net
votes  earned  per  question
. To  ensure  that  these  results  are  not  driven
by outliers or subsequent voters herding on the first upvote, we replicate the anal-
ysis using a binary variable that is equal to 1 if the question receives at least one
upvote, and 0 otherwise. As shown in column 5, the results are robust to this binary

column  4

Δ

(

)

(

)

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019

3423

 specification.20 Consistent with shifting standards, the average change in reputation
and average number of net votes, pooled across both genders, does not significantly
differ between Novice and Advanced accounts.

In summary, we find that in our setting, not only is initial discrimination against
females mitigated by reputation, but the direction of discrimination reverses: females
are favored at higher reputations. Interpreting these findings through the lens of the
theoretical  framework,  our  results  suggest  that  initial  discrimination  is  driven  by
belief-based partiality with bias.

Robustness Checks.—The forum provided us with a proprietary dataset that con-
tains  additional  information  about  the  evaluators  in  our  experiment.  The  dataset
uniquely identifies the users who evaluated our content
i.e., voted on question and
answer posts in our experiment
, and provides their historical activity on the forum.
These data allow us to conduct further robustness checks and to explore the typical
voting behavior of evaluators who interacted with our posts to determine whether
the population of users who evaluated our posts is similar across groups.

(

)

We first use these data to test whether our results are robust to excluding repeat
votes from evaluators who interacted with our posts more than once. We restricted
the voting data to the first vote from each evaluator on a post in our experiment, and
re-ran the analyses from Tables 1 and 2. Our findings are robust to excluding these
repeat votes. The results are presented in online Appendix C.2.

We also explored whether the users who evaluated questions in our experiment
are  similar  to  the  users  who  evaluated  answers. To  determine  whether  users  spe-
cialize in the type of content they evaluate by either evaluating mostly questions or
mostly answers, or whether most users evaluate both, we tabulated each user’s total
number  of  votes  by  content  type,  and  calculated  the  proportion  of  a  given  user’s
votes  that  were  cast  on  questions  versus  answers. The  proportions  are  very  simi-
lar: on average, 48 percent of a user’s votes were cast on questions and 52 percent
were  cast  on  answers,  with  a  standard  deviation  of  0.21. This  suggests  that  most
users evaluated questions and answers in fairly equal proportions. We also examined
whether the users who evaluated our content differed in their reputation levels and
inferred genders, depending on the type of post.21 Summary statistics are presented
in online Appendix C.3; we found no significant differences in the characteristics of
voters evaluating different types of posts.

D. Observational Data

Next, we analyze an observational dataset from the forum. We estimate relevant
population statistics and use these estimates to evaluate alternative potential expla-
nations for the documented discrimination reversal, including differential attrition
by gender, gender differences in the variance of the ability distributions and auto-
correlation in the quality of posts. We also explore gender differences in evaluations
for all users who have a reputation within the range of our experiment and compare
these differences to those found in our experiment.

20 Results are also robust to winsorizing the dependent variable at 5 percent or 10 percent.
21 Section IID outlines the process of inferring gender from a username.

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 103424

(

 and posting behavior
)

Description  of  Data.—The  observational  dataset  is  compiled  and  made  avail-
e.g., reputations, user-
(
e.g., number of question and answer posts

able by the forum. It contains information on the attributes
names, location
)
of 315,792 users from July 2010 to March 2017. We excluded all content posted as
part of our experiment. To code gender, we ran an algorithm developed by Vasilescu,
Capiluppi, and Serebrenik
see online
(
. Each username is classified as
Appendix C.4.1 for a description of this algorithm
“male,” “female,” or “x”
. In our sample, the gen-
when gender cannot be inferred
der was resolved for 55 percent of accounts, which we used in the analyses. Of these
accounts, 19 percent were classified as “female” and the remaining 81 percent were
classified as “male.” Of accounts that had less than 100 reputation points, 21 percent
were classified as “female”; of accounts that had between 100 and 240 reputation
points—the Advanced range used in our experiment —13 percent were classified as
female.

 to classify the gender of the usernames
(

2014

)

)

)

(

Attrition.—We studied posting behavior of users to determine whether there is
differential  attrition  based  on  gender. To  do  so,  we  created  a  panel  dataset  of  up
to the first ten posts for each user, including whether each post was a question or
an  answer  and  the  amount  of  reputation  earned  on  the  post.22  For  each  user,  we
observed whether their first post was followed by a second post, whether their sec-
ond post was followed by a third post, and so on. Differential attrition will lead to
gender differences in the likelihood of observing a subsequent post conditional on
receiving similar evaluations on the prior post.

We first examined whether there was differential attrition by gender following the
first post. We ran a probit regression, regressing a dummy for whether a user gener-
ated a second post on the inferred gender of the username, the log of the reputation
earned on the first post and their interaction, both pooling question and answer posts
and analyzing each separately. We also split the reputation earned on the first post
into quartiles and ran a similar regression. Neither the gender variable nor the inter-
action with reputation or reputation quartile is significant in any of these specifica-
tions. This suggests that female users were no less likely than male users to generate
a second post conditional on a similar first post
see online Appendix Tables 6 and
. We repeated a similar analysis to study differential attrition by gender following
7
)
. These results mirror
the second through ninth posts
the results following the first post: neither the gender variable nor the interaction
with reputation is significant in subsequent periods.

see online Appendix Table 8

(

)

(

Next,  we  ran  a  pooled  analysis  on  all  posts  in  our  panel.  In  order  to  compare
attrition rates for males and females with similar evaluation histories, we created
a  variable  corresponding  to  the  total  reputation  earned  on  all  previous  posts.  For
example,  when  looking  at  the  likelihood  of  a  fourth  post,  total  reputation  earned
is the sum of the reputation earned on the third, second, and first posts. We ran a
probit regression, regressing a dummy for whether a user generated a post  t  on the
gender dummy, the log of the total reputation earned on posts 1 through t
1, their

−

22 The mean number of total posts per user for users in our relevant reputation range

i.e., a reputation of up to
 is 4.29, with a standard devision of 4.66. Therefore, we restricted attention to a user’s first

(

250 at time of posting
10 posts.

)

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019
3425

interaction, and a dummy of whether the previous post was a question. In two of the
three specifications, we also controlled for how many posts it took to generate this
total reputation. Neither the gender variable nor the interaction with total reputation
is significant in any of these specifications

see online Appendix Table 9

(
Taken together, these results suggest that attrition is similar for males and females

.
)

at the post histories that are relevant for our experiment.

Variance.—The observational data  also allow us to examine whether there are
differences in variances of the ability distributions by gender. Since we did not find
evidence for discrimination on answers, we use the evaluations of answers posted
to new accounts to proxy for underlying ability. We then examine whether there are
differences in the variance of these evaluations by gender. Running Levene’s test of
equal variances on the distributions of reputation points per first answer post
Δ
(
0.41  using the mean,  p
reveals no significant differences by gender
  =
using the median,  p

 p
(
0.46  using the 10 percent trimmed mean

 Rep
)
0.48

  =

.

  =

)

Autocorrelation.—As we outline theoretically in online Appendix C.4.3, negative
autocorrelation in the error process for quality could potentially lead to a discrim-
ination reversal in a correctly specified model. We studied the dynamic pattern of
evaluations to determine whether such negative autocorrelation is present empiri-
cally. We compiled a panel dataset consisting of all answer posts by users who had a
reputation between 1 and 250 at the time of posting, which is the relevant reputation
range for our experiment. We used the Wooldridge test for serial correlation in panel
data
. We  first  ran  a  random  effects  regression,  regressing  the
)
reputation earned on an answer post on a gender dummy, then tested the estimated
residuals for autocorrelation. We did not find evidence for significant autocorrela-
tion.  We  used  a  similar  method  for  question  posts  and  also  find  no  evidence  of
significant negative autocorrelation. See online Appendix C.4.3 for a more detailed
description of the analysis.

Wooldridge  2010

(

.

see online Appendix C.4.4 for details
(

Gender Differences in Evaluations.—We also use the observational data to exam-
ine how evaluations of posts vary with reputation, inferred gender of the user and
type of post. As in our experiment, we focus on the evaluation of questions posted
to novice and advanced accounts, and the evaluation of answers posted to novice
accounts. We define posting to novice and advanced accounts similar to the experi-
ment

)
This  analysis  comes  with  several  important  caveats.  First,  there  is  the  obvious
endogeneity problem that stems from not being able to control for the quality of
question posts. Second, there may be gender-based selection between the novice and
advanced accounts. Although the above analysis suggests there is little evidence of
differential attrition conditional on receiving similar evaluations on prior posts, male
and female users may still face different evaluation thresholds early on. In fact, our
experimental results show this to be likely. Finally, the number of posts that gener-
ated a user’s reputation is relevant for inferring ability, as different numbers of posts
can  result  in  similar  reputations. We  attempt  to  address  these  caveats  by  running
different specifications of the regression model, e.g., controlling for number of posts
required to attain advanced status.

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 10

3426

Keeping these caveats in mind, we run regression analogous to Tables 1 and 2 using
the reputation points earned per post
 as the dependent variable. These results
 Rep
)
Δ
(
are  presented  in  online Appendix Tables  10–12. The  evaluation  patterns  by  gender
across the different types of posts are similar to those documented in the experiment,
although the effect sizes vary depending on the specification. We document three main
findings:
 ques-
 no significant evidence of gender discrimination on answers,
i
)
)
(
tions posted by novice accounts with female usernames tend to earn fewer reputation
points than those posted by novice accounts with male usernames, and
 questions
)
posted  to  advanced  accounts  with  female  usernames  tend  to  earn  more  reputation
points than those posted to advanced accounts with male usernames.

iii
(

ii
(

Stereotypes.—Finally, we use the observational data to explore how the “repre-
sentativeness” heuristic can lead to biased stereotypes in our setting. We examine the
distribution of users’ evaluations per answer post, and show how even mild belief
distortions due to “representativeness” significantly magnify small underlying per-
formance differences between males and females. See online Appendix D for details.

III.  Discussion and Conclusion

i

(

)

ii
(

 how it evolves dynamically, and
)

In this paper, we propose a method for identifying the source of discrimination
based on
 how it responds to the degree of
subjectivity in judgment. We develop a theoretical model in which evaluators learn
about  a  worker’s  ability  through  other  evaluators’  assessments  of  previous  tasks.
We show that the observable patterns of discrimination along these two dimensions
depend critically on the underlying source, which we term partiality. The theoretical
analysis yields an impossibility result: discrimination does not dynamically reverse
if  it  is  driven  by  correctly-specified  belief-based  partiality.  In  contrast,  we  show
that a reversal can occur if some evaluators hold biased stereotypes, while others
are aware of the bias and account for it when learning from prior evaluations. We
also show that discrimination driven by preference-based partiality remains constant
with respect to the level of subjectivity in judgment, while discrimination driven by
belief-based partiality decreases as judgment criteria becomes more objective.

i

(

We present results from a field experiment exploring discrimination along these
two dimensions. We post questions and answers on an online forum to accounts we
created that exogenously vary in the gender of the usernames and the reputation on
the  forum. We  document  three  main  results:
  significant  gender  discrimination
)
exists at the initial stage, in the form of less reputation earned per post and fewer
votes  per  post  on  questions  posted  by  low  reputation  female  accounts  relative  to
 significantly less gender dis-
questions posted by low reputation male accounts;
(
crimination at the initial stage for answers, where judgment of quality is less sub-
 discrimination reverses for questions at more
jective relative to questions; and
advanced stages, in that more reputation is earned and more votes are received on
questions posted to high reputation female accounts relative to high reputation male
accounts. We complement the experimental results with an analysis of observational
data from the forum. We use an algorithm to infer gender from username and run
a parallel analysis of how discrimination varies with type of post and user reputa-
tion. This provides additional evidence to support the main findings outlined above.

iii

ii

)

(

)

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019
3427

Taken together, our empirical results are consistent with discrimination driven by
belief-based partiality with some form of misspecification.

The  source  of  discrimination  has  important  implications  for  policies  that  aim
to  reduce  discrimination.  Suppose  a  policymaker  cares  about  both  efficiency  and
“fairness,” defined as equal treatment for equal quality of output. If discrimination is
driven by belief-based partiality with incorrect beliefs, the welfare criterion is clear:
incorrect  initial  beliefs  lead  to  suboptimal  and  unfair  choices,  relative  to  correct
beliefs. Therefore, campaigns that aim to correct initial beliefs will improve choices
along both dimensions, as will designing more objective measures of quality.

)

1993

The  findings  on  dynamics  also  highlight  the  pernicious  effects  of  incorrect
beliefs  about  group-based  differences  in  initial  evaluation  standards.  Kravitz  and
Platania
 conducted a survey on beliefs about affirmative action policies. The
(
authors found that the majority held incorrect beliefs. Respondents viewed affirma-
tive action policies as being much more widespread
required of all organizations
)
(
and as lowering evaluation standards to a much greater extent than is actually the
case.  Such incorrect beliefs can perpetuate inequality in outcomes, despite mem-
bers of disadvantaged groups exceeding earlier standards and earning the relevant
credentials. For example, prospective employers judging the education credentials
of a minority candidate may discount them, relative to the same credentials from a
non-minority  candidate,  if  they  believe  that  the  minority  candidate  faced  a  lower
standard to earn them. In this case, policies that remedy incorrect beliefs about ini-
tial evaluation standards will be particularly effective in mitigating discrimination
down the road. Other policies, such as oversampling from discriminated groups at
the initial stages, may also lead to more equal representation without exacerbating
incorrect beliefs about evaluation standards.

Appendix

Throughout  this  section,  let

signal conditional on ability. We will also use the notation
and
)  +  τ ϵ  )
of the belief about ability and quality, respectively, at time  t .

t
)   ≡   τ a   (

)   τ ϵ  / ( τ a   (

 τ q   (

t

t

 τ ϵη    ≡   τ η    τ ϵ  / ( τ η   +  τ ϵ  )
)   τ ϵη
 , which we show in Lemma 1 denotes the precision

   denote  the  precision  of  the
)   ≡   τ a   +  (

1
 −

 τ a   (

t

t

5

PROOF OF PROPOSITION 1:
 ˆ
 ˆ
h
D
 . From
  if and only if
,
   F
   M    ≠    μ
 1
  μ
 (
 ˆ
 ˆ
c
s
h
 , initial discrimination is equal to  D
  for
,
0  and
 F
   M
   F    =    μ
 1  )   =
 1
 (
  μ
 . In a model with both  preference-based
 , which is constant with respect to

From
, it is clear that
(
|
)
c
, if
4
 F    >
)
(
s
all
and belief-based partiality, initial discrimination is equal to

  is decreasing in

 1    ∈  ℝ

s
 1  ) |

 τ η

 τ η

s

Taking the limit,

 D

,
 1

 τ q
 ˆ
 ˆ
c
 _  τ q   +  τ η      (  μ
   F  )  +
   M   −   μ
 1  )   =
c
c
s
 , which is nonzero if and only if
,
 F    ≠
 F
 1  )   =
 1
The following lemma is used in the proofs of Propositions 2 and 3.

h
 (
D

  τ η  →∞

h
 (

lim

 F  .

0 .

∎

LEMMA 1: Suppose an evaluator has a normally distributed subjective prior dis-
 ˆ
  for a worker of gender  g , has no
  and precision
tribution of ability with mean
 μ

 τ a

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 10

3428

a

preference-based partiality, and believes that all other evaluators are also this type.
2 ,  the  subjective  posterior  distribution  of
   for   t
Then  following  any  history
h
 t
  is normally distributed with mean
h
f
ability
 t  )
 |
t
1
 ˆ
 ˆ
h
v
s
,
−
 n
   +  τ ϵη    ∑ n
 τ a   μ
1
 (
   (
  μ
=
   ____________________
t
1
 τ a   +  (
)   τ ϵη
 −

,
 n  )

  ≥

A1

 a   (

)

n

)

(

 ˆ
h
 t  )   ≡
   (
 μ
t
1
 −

)   τ ϵη

 , where

and precision

t

 τ a   (

)   ≡   τ a   +  (

A2

)

(

 s

 (

v,

 ˆ
h
   (
  μ

,
 t  )

t

)   ≡   (

t

 τ q   (
)  +  τ η
v
 _  τ η
 )

 −  (

t
 τ q   (
)
 ˆ
h
 _  τ η     )  μ
   (

 t  )

t

t

t
 τ q   (

)  +  τ ϵ  )

)   ≡   τ a   (

)   τ ϵ  / ( τ a   (

  is the precision of quality at time  t .

is the signal required to receive evaluation  v  at time  t  when the evaluator has belief
 ˆ
  and
h
 t  )
   (
μ
PROOF:
h
a
f
  denote the subjective posterior distribution of ability following his-
Let
 a   (
)
 |
a
s
f
tory  h  and
  denote the signal distribution conditional on ability.
 s   (
)
 |
Suppose  an  evaluator  has  a  normally  distributed  prior  distribution  of  ability
a
 , no preference-based partiality, and believes
a
a
f
  is nor-
 , so
 +  ϵ t   +  η t
 s   (
)
 |
, conditional on observing
4
)

f
 a   (
s
that all other evaluators are also this type. Recall
 t    =
mally distributed with mean  a  and precision
 . From
(
s
 , the first evaluation is
signal
 1

 ˆ
  and precision
 , with mean
 μ

h
 1  )
 |

 τ ϵη

 τ a

s

A3

)

(

v
 1    =

 ˆ
s
 τ q   μ
 1
   +  τ η
 _  τ q   +  τ η     .

Therefore, the distribution of first period evaluations conditional on ability, denoted
 ˆ
a
 τ q   μ
   +  τ η
h
v
 _  τ q   +  τ η
a,
f
   and  precision
 ,
 v   (
 1  )
 |
2
2
 ˆ
v
s
s
v
s
 .  It  is  possible  to  back  out
 ,
1
,
,
 ,
   from  observing
  ( τ q   +  τ η  )
 1
 1    =
 1
 1
   τ ϵη  / τ  η
)
  μ
 (
,
A2
where from
)
(

is  normally  distributed  with  mean

A4

)

(

 ˆ
v
 s
,
,
 1
  μ
 (

1
)   =   (

 τ q   +  τ η
v
 _  τ η
 1   −  (
 )

 τ q
 ˆ
 _  τ η    )  μ
  .

v
h
Consider the posterior distribution of ability following history
 1  )
 2    =   (

 . From

Bayes’ rule,

a

f
 a   (

h
 2  )   =
 |

f
h
a,
f
v
 a   (
 v   (
 1  )
 1   |
   ___________________
  =
f
h
a
v
f
,
∞
 a   (
 v   (
 1  )
 1   |
 ∫ −∞

h
a
 1  )
 |
h
a
 1  )
′ |

da

′

′

a

 ˆ
v
s
,
,
 1
  μ
 (
 ˆ
v
s
,
,
 1
  μ
 (

f
f
a
h
1
 a   (
 s   (
 1  )
 |
)
)  |
   ______________________
h
a
f
a
f
1
∞
 a   (
 s   (
 1  )
′ |
′)
)  |
 ∫ −∞
follows

da

  ,

′

where

the
 τ q   +  τ η
s
f
 _  τ η     )
 s   (
=   (
 (
f
mal likelihood function. Since

 ˆ
,
  μ

v,

equality

h
second
 1  )
a
 . The normal distribution is conjugate to itself for a nor-
1
)
)  |
f
h
a
  is also nor-
  and
 s   (
 a   (
 1  )
 |
 ˆ
 ˆ
v
s
1
,
,
 τ a   μ
 1
  μ
 (
   +  τ ϵη
  ___________  τ a   +  τ ϵη

f
a
  are normal,
)
 |
)
  and precision

h
 a   (
 2  )
 |
 .
)   =   τ a   +  τ ϵη

v
f
 v   (

from

 τ a   (

a,

 |

a

2

s

 2  )   =

Given the normality of the posterior belief about ability, we can define the eval-
uation  and  belief-updating  processes  recursively.  Suppose  that  the  distribution  of
h
  and precision
ability following history
 t  )

 ˆ
h
  is normally distributed with mean
 t
   (
 μ

 ˆ
h
mal with mean
   (
 μ

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019

3429

 . The evaluation process in period  t
)

t
 τ a   (
s
q
  conditional on observing signal
tion of quality
 t
 ˆ
s
t
h
E ˆ
 t
 t  )  +  τ η
 τ q   (
   (
)  μ
s
q
t
mean
  and precision
  _  τ q   (
 t  ]   =
 τ q   (
   [
)  +  τ η
t
s
 , the evaluation in period  t  is equal to
ditional on observing signal
 t

1 . The distribu-
  =
h
  is normal with
  and history
 t
 t
)  +  τ η

 . Analogous to
(

1  is analogous to  t

h
,
 t
 t   |

, con-

  >

A3

)

A5

)

(

v
 t    =

t

 ˆ
s
h
 τ q   (
 t  )  +  τ η
   (
)  μ
  ____________
t
 τ q   (
)  +  τ η

 t
 .

v
Inverting this expression, the signal required to receive evaluation
  is
 t

t

t

A6

)

(

t
 τ q   (
 τ q   (
)  +  τ η
)
 ˆ
 ˆ
h
v
h
v
 s
,
 _  τ η     )  μ
 _  τ η
 t
 t   −  (
 (
   (
  μ
   (
 )
. Belief-updating is also analogous to  t
A2
1 , the
  =
v
  is normally distrib-
,
 t  )
 t

which is equal to
h
posterior distribution of ability following history
uted with mean

h
1    =   (

)   ≡   (

1 . For  t

,
 t  )

  >

,
 t  )

 t
+

(

)

A7

)

(

 ˆ
h
   (
 μ

 t
+

1  )   ≡

t
t
1
and precision
)   =   τ a   (
 τ a   (
)  +  τ ϵη  .
 +
 ˆ
 ˆ
h
1
  and
Initializing
 τ a   (
 1  )   =   μ
   (
 μ
 ˆ
h
  yields solution
  and
 t  )
)
   (
μ
A8

 τ a   (

t

)   =   τ a

t

 ˆ
h
   (
)  μ

 ˆ
h
v
s
,
 t  )  +  τ ϵη
 τ a   (
 t
   (
  μ
 (
   ___________________
t
 τ a   (
)  +  τ ϵη

,
 t  )

)

t

 , and solving the recursive expressions for

(

)

 ˆ
h
   (
 μ

A9

)

(

 t  )   =
t
 τ a   (

t
1
 ˆ
 ˆ
h
v
s
,
−
 n
   +  τ ϵη    ∑ n
 τ a   μ
1
   (
  μ
 (
=
   ____________________
t
1
 τ a   +  (
 −
)   τ ϵη
 ,
1
)   τ ϵη
 −
1 . Therefore, when the prior distribution of ability is normal, the distribu-
 ˆ
h
h
  and
 , is also normal with mean
 t  )
 t  )
   (
 μ
 |

for  t
f
h
 , i.e.,
tion of ability following history
 t
precision

t
)   =   τ a   +  (

,
 n  )

  >

 a   (

)
 ,

n

a

t
 τ a   (

 .
)
PROOF OF PROPOSITION 2:

∎

Suppose  there  is  a  single  type  of  evaluator  with  belief-based  partiality  and  no
 ˆ
 ˆ
preference-based  partiality.  Given  initial  beliefs
 t  )
   M
   F    <    μ
  μ
denote the subjective average ability of a female and male worker, respectively, fol-
h
lowing history

 ˆ
h
   and
   M   (
 t  )
  μ

 ˆ
h
 ,  let
   F   (
  μ

 . We proceed by a series of lemmas.
 t

 ˆ
 ˆ
 , there is no belief reversal between
 , then for all
v
h
h
LEMMA 2: If
 t
 t  )
 t  )   <    μ
   F   (
   M   (
  μ
 ˆ
 ˆ
 ,  and  the  difference  in  beliefs  about
h
h
1 ,
periods   t   and   t
   M   (
 t
   F   (
1  )
1  )   <    μ
  μ
 +
+
 ˆ
h
1 ,
average  ability  decreases  between  periods   t   and   t
   M   (
1  )
  μ

 ˆ
h
   F   (
1  )  −   μ

 +

 t
+

 t
+

 t
+

 ˆ
h
   F   (
 t  )  −   μ

 .
 t  )

 ˆ
h
   M   (
<    μ
PROOF:

 ˆ
h
Suppose
   F   (
  μ

 ˆ
h
   M   (
 t  )   <    μ

 . The difference in signals required for a male and a
 t  )

v
  is
female worker to receive evaluation
 t

 ˆ
 s
h
v
,
   M   (
 t
 (
   μ

,
 t  )

t

s
)  −

 ˆ
h
v
,
   F   (
 t
   μ
 (

,
 t  )

t

t
 τ q   (
)
 ˆ
h
 _  τ η     )  (  μ
   M   (

)   =  − (

 ˆ
h
   F   (
 t  )  −   μ

,
 t  ) )

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 10

3430

t

v,

where   s
A7
)
 (
v
  is
difference in the belief about posterior average ability following evaluation
 t

 ˆ
h
. Therefore,  given
   g   (
  μ
)

   is  defined  in
)

   defined  in

 ˆ
,
  μ

1  )

A2

 t
+

(

(

,  the

A10

)

(

 ˆ
h
   M   (
  μ

 ˆ
h
   F   (
1  )  −   μ

 t
+

 t
+

1  )   =   (

 t  ) )

 ˆ
h
   F   (
 t  )  −   μ

t
 τ a   (
)
 ˆ
h
 _
   M   (
  )  (  μ
t
 τ a   (
)  +  τ ϵη
 τ ϵη
 ˆ
h
v
  )  (s
,
 _
   M   (
 t
   μ
 (
+  (
t
 τ a   (
)  +  τ ϵη
t
t
)  −  τ ϵη    τ q   (
 τ a   (
 ˆ
h
  _____________
   M   (
 )  (  μ
t
 τ a   (
)  +  τ ϵη

)  /  τ η

=   (

,
 t  )

t

s
)  −

 ˆ
h
v
,
   F   (
 t
   μ
 (

,
 t  )

t

) )

 ˆ
h
   F   (
 t  )  −   μ

 t  ) ) .

t

t

) / τ η    >

0 ,  which  is  equivalent  to

This  is  positive  if
 τ a   (
Therefore,

)  −  τ ϵη    τ q   (
2
)  ( τ ϵ   +  τ η  )   >   τ  ϵ
 ˆ
 ˆ
h
h
   F   (
 t
   M   (
1  )   >    μ
  μ
+
 ˆ
 ˆ
h
h
   M   (
 t
   F   (
 t
1  )   <    μ
1  )  −   μ
+
+

t
 τ a   (
  +  τ ϵ    τ η   +
 ,  which  always  holds  since  all  precisions  are  positive.
,
)

A10
(
t
 τ ϵη    τ q   (
)
 _
t
)  +  τ ϵη  )   τ η
 ( τ a   (
1,  which always holds since the first term is less than 1 and the second term is

 ˆ
h
   M   (
  μ
<
subtracting a positive number. This establishes part

1
.  From
(
)
t
 τ a   (
)
 _  τ a   (
)  +  τ ϵη     −
t

   if  and  only  if
 t  )

 t
1  )
+
 ˆ
h
   F   (
 t  )  −   μ

 ,  which  establishes  part

2
 τ  ϵ

2

.

)

∎

(

 ˆ
 ˆ
Therefore, given prior beliefs
 , by Lemma 2, the difference in beliefs
   M
   F    <    μ
  μ
about average ability for males and females with the same history decreases across
 ˆ
 ˆ
h
h
h
 . The next lemma estab-
  for all
periods but never reverses, i.e.,
 t
 t  )
   M   (
 t  )   <    μ
   F   (
  μ
lishes that this rules out discrimination reversals.

LEMMA  3:  A  discrimination  reversal  occurs  between  periods   t   and   t
1   if  and
only if the beliefs about average ability of male and female workers reverse between
periods  t  and  t

 +

1 .

 +

PROOF:

 ˆ
h
Given beliefs
   M   (
  μ

 ˆ
h
  and
   F   (
 t  )
  μ

 , from
 t  )
(

A5

, discrimination in period  t  is equal to
)

A11

(

)

 D

h
 (

,
 t

s
 t  )   =   (

t
 τ q   (
)
 ˆ
h
 _
   M   (
  )  (  μ
t
 τ q   (
)  +  τ η

 ˆ
h
   F   (
 t  )  −   μ

 t  ) ) .

Therefore,  discrimination  reverses  between  periods   t   and   t
 ˆ
 ˆ
 ˆ
h
h
h
   F   (
   M   (
   F   (
 t  )   >    μ
1  )   <    μ
  μ
 ˆ
h
h
 , by Lemma 3, there is no discrimination reversal
  for all
Given
 t
 t  )
   F   (
  μ
between any periods  t  and  t

 ˆ
h
  and
   M   (
 t  )
  μ
 ˆ
h
   M   (
 t  )   <    μ

1 . This establishes Proposition 2.

1   if  and  only  if

 , or vice versa.

1  )

 +

 t
+

 t
+

∎

 +

∎

PROOF OF PROPOSITION 3:

a
h
f
   denote  the  subjective  posterior  distribution  of  ability  following  his-
Let
 a   (
)
 |
a
s
tory  h  and
f
  denote the signal distribution conditional on ability. Suppose evalua-
 s   (
)
 |
  with
0,
  and the impartial type
tors are the heuristic type
 θ 1
)
p . Type
 ’s belief about male and female ability evolve as in Lemma
probability  1
 θ 1
 ’s
1, since this type believes that all other evaluators have the same beliefs as it. Type

  with probability  p

  ∈   (

 θ 2

 −

1

 θ 2

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019

3431

 θ 1

  evaluates all workers and type

belief about male ability also evolves as in Lemma 1, since both types have the same
prior belief about male ability. Therefore, type
 θ 2
evaluates male workers in the same way as was previously characterized. The novelty
  evaluates female workers in the second period.
stems from characterizing how type
 θ 2
  updates its belief about a female worker’s abil-
We first characterize how type
v
  observes evaluation

ity after the first evaluation. Suppose an evaluator of type
 1
in period one for a female worker. The evaluator believes that with probability  p ,
it  is  from  a  heuristic  type

 θ 1
 τ q
1
 ˆ
 , and with probability  1
 _  τ η    )   μ
    F
(
 ˆ
signal   s
v
,
,
1
   M
 1
)
 (
   μ
 ˆ
v
s
 . Therefore, the distribution of first period evaluations conditional on
1
,
,
   M
 1
)
   μ
 (

>
ability  a  is a mixture of two normal distributions,

 τ q   +  τ η
v
 _  τ η     )
 1   −
  who observed

1
)   =   (
 θ 2
.  Note   s

 −
 τ q   +  τ η
v
 _  τ η     )
 1   −  (

2
 ˆ
 ˆ
recall
   M
    F
)
   =    μ
  μ

p , it is from an impartial type

   who  observed  signal   s

1
 ˆ
v
,
,
    F
 1
 (
   μ

1
 ˆ
v
,
,
    F
 1
 (
   μ

 τ q
 ˆ
 _  τ η    )   μ
   M

)   =   (

 θ 2

 θ 2

1

(

f

s

v

1
 ˆ
,
    F
   μ

 τ q   +  τ η
 )  (p
 _  τ η

v,

 |

a,

 s   (s
 (

a)  +  (
1
1
)  |

h
 1  )   =   (
  is normally distributed with mean  a  and precision
a
)
 |

a
f
,
 v   (
) )
)  |
f
 . Consider the
where
 s   (
v
h
 . Since the prior belief
posterior distribution of ability following history
 1  )
 2    =   (
 ˆ
f
h
a
f
  is a mixture
  and the likelihood function
  is normal with mean
 a   (
 v   (
   M
 1  )
  μ
 |
of  two  normal  distributions,  the  posterior  belief  will  be  a  mixture  of  two  normal
distributions,

p
 −

h
 1  )

f
 s   (
)

v,
s
 (

 ˆ
,
   M
   μ

 τ ϵη

a,

 |

1

v

f

a

p

 a,2   (

a
 a   (

p
 −

a
 a,2   (

h
,
 2  )
 |

h
 2  )   =
 |

  and  s
1
)

h
1
 2  )  +  (
 |

C
h
 a,2   (
 2  )
f
 _
  )
)  (
h
C
 a   (
 2  )

C
h
 a,1   (
 2  )
f
 _
 a,1   (
  )
 (
h
C
 a   (
 2  )
f
h
a
f
h
a
where
   denote  the  posterior  distributions  of  ability  condi-
   and
 a,1   (
 2  )
 2  )
 |
 |
1
 ˆ
 ˆ
v
v
tional on observing signals  s
,
,
 , respectively, which are both
,
,
   M
    F
 1
 1
 (
)
   μ
 (
   μ
 ˆ
h
normally  distributed  with  corresponding  means
 2  )   ≡
   1   (
  μ
 ˆ
 ˆ
s
v
,
,
 τ a     μ
   M   +  τ ϵη
   M
 1
 (
   μ
  ____________   τ a   +  τ ϵη
1
 ˆ
v
 s   (s
f
h
,
,
    F
 a,1   (
 2  )   ≡   ∫ −∞
 1
 (
   μ
_
1 _
 τ a    τ ϵη
exp
 _  τ a   +  τ ϵη
_
    √
2
 √
π

1
 ˆ
 ˆ
v
s
,
,
1
 τ a     μ
    F
   M   +  τ ϵη
 1
)
 (
   μ
   and
  ____________   τ a   +  τ ϵη
 , and

1
)
,  respectively, and precision  1

2
 ˆ
s
   M  )
 ( τ a     (  μ
  +  τ ϵη

1
 ˆ
v
,
,
    F
 1
   (
   μ

/( τ a   +  τ ϵη  )

a
a)
f
 a   (

 2  )   ≡

h
 1  )
 |

 ˆ
h
   2   (
  μ

1
)  |

  (−

=

0.5

da

C

1

∞

2
1
)
 ˆ
h
−  ( τ a   +  τ ϵη  )   μ
   1     (

2
 ,
 2  )
 ) )

C

h
 a,2   (

∞

1

 ˆ
v
f
s
,
,
   M
 s   (
 1
 2  )   ≡   ∫ −∞
 (
   μ
_
1 _
 τ a    τ ϵη
exp
 _  τ a   +  τ ϵη
_
    √
2
 √
π

=

f
a
 a   (
)
)  |

a

da

h
 1  )
 |

0.5

2
 ˆ
s
 ( τ a     (  μ
   M  )
  +  τ ϵη

  (−

1

 ˆ
v
,
,
   M
 1
   μ
   (

2
)
 ˆ
h
−  ( τ a   +  τ ϵη  )    μ
   2     (

2
 2  )

 ,
 ) )

C

h
 a   (

 2  )   ≡

p

h
C
 a,1   (

 2  )  +  (

1

p
 −

h
C
 a,2   (
)

 2  )

are normalization coefficients.

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 10

3432

We next characterize how type

  updates its belief about a female worker’s qual-
 θ 2
h
q
f
v
h
 , let
  denote the prior distribution
ity in period 2. Given history
 q   (
 1  )
 2    =   (
 2  )
 |
s
h
q
f
  denote the posterior belief about
,
of quality in the second period and let
 q   (
 2  )
 2
 |
a
q
s
h
  is normally distributed
 . Recall
  and signal
quality following
 2    =
 2
 2
h
f
  is a mixture of two normal distributions. The convolution of a normal
and
 2  )
 |
distribution with a mixture of two normal distributions is a mixture of two normal
f
  is a mixture of two normal distributions. Since the
distributions. Therefore,
 q   (
q
f
f
  is also a mixture
  is normally distributed, posterior
likelihood function
 q   (
 s
of two normal distributions:

 ,
 ϵ 2
 +  ϵ 2

h
 2  )
 |

h
,
 2
 |

s
 2  )

a
 a   (

q

f
 q   (

q

h
,
 2
 |

s
 2  )   =

p

h
C
h
C
,
 a,1   (
 q,1   (
 2
 2  )
 2  )
f
  _____________
 q,1   (
   )
 (
s
h
C
h
C
,
 q   (
 a   (
 2  )
 2
 2  )

s

q

h
,
 2
 |

s
 2  )

1

p
 −

+  (

s
h
C
h
C
,
 q,2   (
 a,2   (
 2  )
 2
 2  )
f
  _____________
 q,2   (
   )
)  (
s
h
C
h
C
,
 q   (
 a   (
 2  )
 2
 2  )

q

h
,
 2
 |

s
 ,
 2  )

q

h
s
,
   are  both  normally  distributed  with  corre-
 q,2   (
 2  )
 2
 |
 ˆ
s
h
2
 τ q   (
 2
   1   (
 2  )  +  τ η
 ˆ
)    μ
h
s
  and
  ___________  τ q   (
   q,2   (
 2  )   ≡
  μ
)  +  τ η
2
 , and
2
/( τ q   (
_
2
 τ q   (
)   τ η
exp
 _
2
 τ q   (
)  +  τ η

 ˆ
h
s
 τ q   (
 2
   2   (
 2  )  +  τ η
)    μ
s
 ,
  ___________  τ q   (
 2  )   ≡
)  +  τ η
2

2
2
s
 2  )
 2  )
  +  τ η    (

 ˆ
h
   1     (
)    μ

)  +  τ η  )

 ( τ q   (

  (−

0.5

,
 2

2

2

2
 −  ( τ q   (

 ˆ
h
)  +  τ η  )   μ
   q,1     (

,
 2

2
s
 2  )

 ,
 ) )

s

f
where

h
q
,
 q,1   (
 2  )
 2
 |
 ˆ
h
sponding means
   q,1   (
  μ

,
 2

f
   and

respectively, and precision  1

s
 2  )   ≡

1 _
_
    √
2
 √
π

C

h
 q,1   (

,
 2

h
C
 q,2   (

,
 2

s
 2  )   ≡

1 _
_
    √
2
 √
π

_
2
 τ q   (
)   τ η
exp
 _
2
 τ q   (
)  +  τ η

0.5

2
 ( τ q   (

 ˆ
h
   2     (
)    μ

2
 2  )

2
s
 2  )
  +  τ η    (

  (−

−  ( τ q   (

2

,
 2

2
s
 ,
 2  )
 ) )

 ˆ
h
)  +  τ η  )    μ
   q,2     (
C
h
h
C
 q,2   (
 a,2   (
 2  )
  _____________
)  (
h
C
 a   (
 2  )

s
 2  )

 )

,
 2

C

,
 2

h
 q   (

C
h
h
C
 q,1   (
 a,1   (
 2  )
p
  _____________
 )  +  (
 (
h
C
 a   (
 2  )
are normalization coefficients.

s
 2  )   ≡

s
 2  )

,
 2

1

p
 −

Finally, we compute aggregate discrimination in period two. Consider a female
s
  in the second period. The
  who generates signal
 2

v
 1  )
 2    =   (
  gives this worker evaluation

h
worker with history
impartial type

 θ 2

h
v
 2   (

,
 2

s
,
 2

F
)   =   (

2
 τ q   (
)
h
 _
  ) γ (
2
 τ q   (
)  +  τ η

s

,
 2

 2  )  +  (

 τ η
s
,
 _
 2
  )
2
 τ q   (
)  +  τ η

where

h
γ (

,
 2

s
 2  )   ≡

p

s
h
C
h
C
,
 a,1   (
 q,1   (
 2  )
 2
 2  )
 ˆ
h
  _____________
   1   (
 (
   )    μ
s
h
C
h
C
,
 q   (
 a   (
 2  )
 2
 2  )

1
 2  )  +  (

p
 −

C
h
s
h
C
,
 a,2   (
 q,2   (
 2  )
 2  )
 2
 ˆ
h
  _____________
   2   (
   )   μ
)  (
s
h
C
h
C
,
 q   (
 a   (
 2  )
 2
 2  )

 2  ) .

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019

The heuristic type

  gives this worker evaluation

 θ 1

3433

v

h
 1   (

,
 2

s
,
 2

F
)   =   (

1
 ˆ
h
where  from  Lemma  1,
    F
  (
  μ
evaluation

2
 τ q   (
1
)
 ˆ
h
 _
    F
 2  )  +  (
  (
  )    μ
2
 τ q   (
)  +  τ η
1
1
 ˆ
 ˆ
v
s
,
,
 τ a     μ
    F
    F
 1
 (
   μ
  +  τ ϵη
  ____________   τ a   +  τ ϵη

 2  )   =

 τ η
s
,
 _
 2
  )
2
 τ q   (
)  +  τ η

1
)
 .  Both  types  give  males

s

M

,
 2

,
 2

 v
h
 (

2
 τ q   (
)
 ˆ
h
 _
   M   (
 2  )  +  (
  )    μ
2
 τ q   (
)  +  τ η
 ˆ
 ˆ
v
s
,
,
 τ a     μ
   M
   M   +  τ ϵη
 1
 ˆ
   μ
 (
h
where from Lemma 1,
  ____________   τ a   +  τ ϵη
   M   (
  μ
ination in the second period is equal to

)   =   (

 2  )   =

1

 τ η
s
,
 _
 2
  )
2
 τ q   (
)  +  τ η

)
 . Therefore, aggregate discrim-

 D

h
 (

,
 2

s
 2  )   =

h
v
 (

,
 2

s

,
 2

M

p
)  −

v

h
 1   (

,
 2

s

,
 2

F

)  −  (

1

p
 −

h
v
 2   (
)

,
 2

s
,
 2

F

)

1
 ˆ
h
    F
  (
  μ

1
 2  )  −  (

p
 −

h
) γ (

,
 2

s

 2  ) ) .

=   (

2
 τ q   (
)
 ˆ
h
  )  (  μ
 _
   M   (
2
 τ q   (
)  +  τ η
h
Aggregate  discrimination  reverses  at
 (
 2  )   =

p
 2  )  −

,
 2

s

   if   D
0 ,  as  this  is  the  case  with  no  partiality,  and  at   p

s
0 .  We  know  that
 2  )
h
1 ,
 (
0 , as this is the case with a single type of evaluator with belief-based
  with respect
p –  )

0 ,   D
at   p
  =
s
h
 D
,
 2  )   >
 2
 (
partiality from Proposition 2. Therefore, if the derivative of  D
to  p  is negative at  p
before becoming positive. This derivative simplifies to showing that

0 , discrimination will become negative for an interval   (0,

s
 2  )   <

s
 2  )

  =

  =

h
 (

h
 (

,
 2

,
 2

,
 2

A12

(

)

 1
  <   (

2
1
 τ  ϵ
 _____________
  )  (
 ( τ ϵ   +  τ η  )  ( τ a   +  τ ϵ  )

From the expressions above,

h
h
C
C
 q,1   (
 a,1   (
 2  )
  _____________
 +
h
C
h
C
 q,2   (
 a,2   (
 2  )

s
 2  )
s
 2  )

,
 2
,
 2

  ) .

1

2

+

0.5

0.5

exp

  (−

,
 2
,
 2

 τ ϵη   (s

s
 2  )
s
 2  )

1
 ˆ
v
,
,
    F
 1
   (
   μ

h
C
h
C
 q,1   (
 a,1   (
 2  )
  _____________
    =
h
C
h
C
 q,2   (
 a,2   (
 2  )

2
s
1
)
 −
 ˆ
h
) )  (  μ
 ( τ a   +  τ ϵη   −  τ q   (
   1     (
 ˆ
s
h
,
)  +  τ η   (  μ
 ( τ q   (
   q,1     (
 2
s
v
  and decreasing in
which is increasing in
 1
 1
s
s
   approaches  infinity.  Therefore,  fixing
 ,  there
approaches  negative  infinity  or
 2
 2
exists a   v –   such that for
v –  ,
v
h
 , there exists
 is satisfied. Similarly, fixing
A12
 1    >
 2
(
s
s
s
 is satisfied. Therefore, for any prior beliefs about
A12
 ,
  such that for
an
 2    <
)
(
¯
¯
ability for each type, it is possible for discrimination to reverse in the second period.
∎

2
 ˆ
v
,
,
 )
   M
 1
   μ
   (
)
2
2
 ˆ
h
 )
 2  )
   2     (
 2  )
  −   μ
2
2
 ˆ
s
h
,
,
 ) ) )
   q,2     (
 2  )
 2
 2  )
  −   μ
v
 , and becomes arbitrarily large as
 2

0.5

+

2

)

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 10

(

)

(

)

3434

Aigner, Dennis J., and Glen G. Cain. 1977. “Statistical Theories of Discrimination in Labor Markets.”

REFERENCES

Industrial and Labor Relations Review 30

2

: 175–87.

Altonji, Joseph G., and Charles R. Pierret. 2001. “Employer Learning and Statistical Discrimination.”

Quarterly Journal of Economics 116

1

: 313–50.

(

)

Anwar, Shamena, and Hanming Fang. 2006. “An Alternative Test of Racial Prejudice in Motor Vehicle

Searches: Theory and Evidence.” American Economic Review 96

1

: 127–51.

Arnold, David, Will Dobbie, and Crystal S. Yang. 2018. “Racial Bias in Bail Decisions.” Quarterly

Journal of Economics 133

4

: 1885–1932.

(

)

Arrow, Kenneth. 1973. “The Theory of Discrimination.” In Discrimination in Labor Markets, edited

by Orley Ashenfelter and Albert Rees, 3–33. Princeton, NJ: Princeton University Press.

Ayalew, Shibiru, Shanthi Manian, and Ketki Sheth. 2018. “Discrimination from Below: Experimental

Evidence on Female Leadership in Ethiopia.” Unpublished.

Bartoš, Vojtech, Michal Bauer, Julie Chytilová, and Filip Matejka. 2016. “Attention Discrimination:
Theory  and  Field  Experiments  with  Monitoring  Information  Acquisition.”  American  Economic
Review 106

: 1437–75.

Beaman, Lori, Raghabendra Chattopadhyay, Esther Duflo, Rohini Pande, and Petia Topalova. 2009.
: 1497–

“Powerful Women: Does Exposure Reduce Bias?” Quarterly Journal of Economics 124
4
(
1540.

)

6
(

)

Becker, Gary S. 1957. The Economics of Discrimination. Chicago: University of Chicago Press.
Bertrand, Marianne, Dolly Chugh, and Sendhil Mullainathan. 2005. “Implicit Discrimination.” Amer-

ican Economic Review 95

2

: 94–98.

(

)

Bertrand, Marianne, and Esther Duflo. 2017. “Field Experiments on Discrimination.” In Handbook of
Economic Field Experiments, Vol. 1, edited by Abhijit Vinayak Banerjee and Esther Duflo, 309–93.
Amsterdam: North-Holland.

Bertrand, Marianne, and Sendhil Mullainathan. 2004. “Are Emily and Greg More Employable than
Lakisha and Jamal? A Field Experiment on Labor Market Discrimination.” American Economic
Review 94

: 991–1013.

Biernat, Monica, Melvin Manis, and Thomas E. Nelson. 1991. “Stereotypes and Standards of Judg-

4
(

)

ment.” Journal of Personality and Social Psychology 60

4

: 485–99.

(

)

Biernat, Monica, Theresa K. Vescio, and Melvin Manis. 1998. “Judging and Behaving toward Mem-
bers of Stereotyped Groups: A Shifting Standards Perspective.” In Intergroup Cognition and Inter-
group Behavior, edited by Constantine Sedikides, John Schopler, and Chester A. Insko, 151–76.
Mahwah, NJ: Lawrence Erlbaum Associates.

Bocart, Fabian Y. R. P., Marina Gertsberg, and Rachel A. J. Pownall. 2018. “Glass Ceilings in the Art

Market.” Unpublished.

Bohren, J. Aislinn, Kareem Haggag, Alex Imas, and Devin G. Pope. 2019. “Inaccurate Statistical Dis-

crimination.” NBER Working Paper 25935.

Bohren,  J.  Aislinn,  and  Daniel  N.  Hauser.  2018.  “Social  Learning  with  Model  Misspecification: A

Framework and a Robustness Result.” Unpublished.

Bohren, Aislinn, Alex Imas, and Michael Rosenberg. 2018. “The Language of Discrimination: Using

Experimental versus Observational Data.” AEA Papers and Proceedings 108: 169-74.

Bohren, J. Aislinn, Alex Imas, and Michael Rosenberg. 2019. “The Dynamics of Discrimination: The-
ory and Evidence: Dataset.” American Economic Review. https://doi.org/10.1257/aer.20171829.
Booth, Alison L., Marco Francesconi, and Jeff Frank. 1999. “Glass Ceilings or Sticky Floors?” Unpub-

lished.

Bordalo,  Pedro,  Katherine  Coffman,  Nicola  Gennaioli,  and  Andrei  Shleifer.  2016.  “Stereotypes.”

Quarterly Journal of Economics 131

4

: 1753–94.

(

)

(

)

Coate, Stephen, and Glenn C. Loury. 1993. “Will Affirmative-Action Policies Eliminate Negative Ste-

reotypes?” American Economic Review 83

5

: 1220–40.
)

(

Coffman, Katherine Baldiga. 2014. “Evidence on Self-Stereotyping and the Contribution of Ideas.”

Quarterly Journal of Economics 129

4

: 1625–60.

Dana, Jason, Roberto A. Weber, and Jason Xi Kuang. 2007. “Exploiting Moral Wiggle Room: Experi-

ments Demonstrating an Illusory Preference for Fairness.” Economic Theory 33

: 67–80.

Danilov, Anastasia, and Silvia Saccardo. 2017. “Discrimination in Disguise.” Unpublished.
Ewens, Michael, Bryan Tomlin, and Liang Choon Wang. 2014. “Statistical Discrimination or Preju-

1
(

)

dice? A Large Sample Field Experiment.” Review of Economics and Statistics 96

Fang,  Hanming,  and  Andrea  Moro.  2011.  “Theories  of  Statistical  Discrimination  and  Affirmative
Action: A Survey.” In Handbook of Social Economics, Vol. 1, edited by Jess Benhabib, Matthew O.
Jackson, and Alberto Bisin, 133–200. Amsterdam: North-Holland.

1

: 119–34.
)

(

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019Fershtman, Chaim, and Uri Gneezy. 2001. “Discrimination in a Segmented Society: An Experimental

3435

Approach.” Quarterly Journal of Economics 116

1

: 351–77.
)

(

Fiske, Susan T. 1998. “Stereotyping, Prejudice, and Discrimination.” In The Handbook of Social Psy-
chology, Vol. 1, edited by Daniel T. Gilbert, Susan T. Fiske, and Gardner Lindzey, 357–411. Bos-
ton: McGraw-Hill.

Fiske,  Susan T.,  Donald  N.  Bersoff,  Eugene  Borgida,  Kay  Deaux,  and  Madeline  E.  Heilman.  1991.
“Social Science Research on Trial: Use of Sex Stereotyping Research in Price Waterhouse v. Hop-
kins.” American Psychologist 46

: 1049–60.

10

Fiske, Susan T., and Shelley E. Taylor. 1991. Social Cognition. New York: McGraw-Hill Education.
Fryer, Roland G. 2007. “Belief Flipping in a Dynamic Model of Statistical Discrimination.” Journal of

(

)

Public Economics 91

5–6

: 1151–66.

(

)

Fryer, Roland, and Matthew O. Jackson. 2008. “A Categorical Model of Cognition and Biased Deci-

sion-Making.” B.E. Journal of Theoretical Economics 8

1

: Article 1935–1704.

Gneezy, Uri, John List, and Michael K. Price. 2012. “Toward an Understanding of Why People Dis-
criminate: Evidence from a Series of Natural Field Experiments.” NBER Working Paper 17855.
Goldin, Claudia, and Cecilia Rouse. 2000. “Orchestrating Impartiality: The Impact of ‘Blind’ Audi-

tions on Female Musicians.” American Economic Review 90

4

: 715–41.

Gornall, Will, and Ilya A. Strebulaev. 2018. “Gender, Race, and Entrepreneurship: A Randomized Field
Experiment on Venture Capitalists and Angels.” https://papers.ssrn.com/sol3/papers.cfm?abstract_
id=3301982

accessed August 16, 2019

.

Greenwald, Anthony G., Debbie E. McGhee, and Jordan L. K. Schwartz. 1998. “Measuring Individ-
ual Differences in Implicit Cognition: The Implicit Association Test.” Journal of Personality and
Social Psychology 74

: 1464–80.

)

(

Groot, Wim, and Henriëtte Maassen van den Brink. 1996. “Glass Ceilings or Dead Ends: Job Promo-

6
(

)

(

)

(

)

tion of Men and Women Compared.” Economics Letters 53

2

: 221–26.

Kelley, Harold H. 1973. “The Process of Causal Attribution.” American Psychologist 28
: 107–28.
Knowles, John, Nicola Persico, and Petra Todd. 2001. “Racial Bias in Motor Vehicle Searches: Theory

2
)

(

and Evidence.” Journal of Political Economy 109

1

: 203–29.
)

(

Kravitz, David A., and Judith Platania. 1993. “Attitudes and Beliefs about Affirmative Action: Effects

of Target and of Respondent Sex and Ethnicity.” Journal of Applied Psychology 78

: 928–38.

Leslie, Lisa M., Colleen Flaherty Manchester, and Patricia C. Dahm. 2017. “Why and When Does the
Gender Gap Reverse? Diversity Goals and the Pay Premium for High Potential Women.” Academy
of Management Journal 60

: 402–32.

2

Lewis, Gregory B. 1986. “Gender and Promotions: Promotion Chances of White Men and Women in

(

)

6
(

)

Federal White-Collar Employment.” Journal of Human Resources 21

3

: 406–19.

List, John A. 2004. “The Nature and Extent of Discrimination in the Marketplace: Evidence from the
1
)
Lundberg,  Shelly  J.,  and  Richard  Startz.  1983.  “Private  Discrimination  and  Social  Intervention  in

Field.” Quarterly Journal of Economics 119

: 49–89.

(

(

)

(

)

Competitive Labor Markets.” American Economic Review 73

3

: 340–47.
)

(

Mengel, Friederike, Jan Sauermann, and Ulf Zölitz. 2019. “Gender Bias in Teaching Evaluations.”

Journal of the European Economic Association 17

2

: 535–66.

(

)

Milgrom, Paul. 1981. “Good News and Bad News: Representation Theorems and Applications.” Bell

Journal of Economics 12

2

: 380–91.

(

)

Milkman, Katherine L., Modupe Akinola, and Dolly Chugh. 2012. “Temporal Distance and Discrimi-

nation: An Audit Study in Academia.” Psychological Science 23

Moss-Racusin, Corinne A., John F. Dovidio, Victoria L. Brescoll, Mark J. Graham, and Jo Handels-
man.  2012.  “Science  Faculty’s  Subtle  Gender  Biases  Favor  Male  Students.”  Proceedings  of  the
National Academy of Sciences 109

: 16474–79.

41

Olson, James M., Robert J. Ellis, and Mark P. Zanna. 1983. “Validating Objective versus Subjective
Judgment: Interest in Social Comparisons and Consistency Information.” Personality and Social
Psychology Bulletin 9

: 427–36.

3

Parsons, Christopher A., Johan Sulaeman, Michael C. Yates, and Daniel S. Hamermesh. 2011. “Strike
: 1410–35.
)
Petersen, Trond, and Ishak Saporta. 2004. “The Opportunity Structure for Discrimination.” American

Three: Discrimination, Incentives, and Evaluation.” American Economic Review 101
(

4

(

)

(

)

7

: 710–17.
)

(

Journal of Sociology 109

4

: 852–901.

Phelps, Edmund S. 1972. “The Statistical Theory of Racism and Sexism.” American Economic Review

62

4

: 659–61.

(

)

Price,  Joseph,  and  Justin Wolfers.  2010.  “Racial  Discrimination  among  NBA  Referees.”  Quarterly

Journal of Economics 125

4

: 1859–87.

Pronin, Emily, Daniel Y. Lin, and Lee Ross. 2002. “The Bias Blind Spot: Perceptions of Bias in Self

versus Others.” Personality and Social Psychology Bulletin 28

: 369–81.

3
(

)

(

)

(

)

BOHREN ET AL.: THE DYNAMICS OF DISCRIMINATION: THEORY AND EVIDENCEVOL. 109 NO. 10(

)

3436

Reuben,  Ernesto,  Paola  Sapienza,  and  Luigi  Zingales.  2014.  “How  Stereotypes  Impair  Women’s

Careers in Science.” Proceedings of the National Academy of Sciences 111

12

: 4403–08.

(

)

Riach, Peter A., and Judith Rich. 2006. “An Experimental Investigation of Sexual Discrimination in
Hiring in the English Labor Market.” B.E. Journal of Economic Analysis and Policy: Advances in
Economic Analysis & Policy 6

: 1–20.

2

Rosette, Ashleigh Shelby, and Leigh Plunkett Tost. 2010. “Agentic Women and Communal Leadership:
How Role Prescriptions Confer Advantage to Top Women Leaders.” Journal of Applied Psychol-
ogy 95

: 221–35.

2

(

)

Ross,  Lee,  David  Greene,  and  Pamela  House.  1977.  “The  ‘False  Consensus  Effect’: An  Egocentric
Bias in Social Perception and Attribution Processes.” Journal of Experimental Social Psychology
13

: 279–301.

3

Sarsons, Heather. 2017. “Interpreting Signals in the Labor Market: Evidence from Medical Referrals.”

Unpublished.

Schwartzstein, Joshua. 2014. “Selective Attention and Learning.” Journal of the European Economic

(

)

Association 12

6

: 1423–52.
)

(

Snyder, Melvin L., Robert E. Kleck, Angelo Strenta, and Steven J. Mentzer. 1979. “Avoidance of the
Handicapped: An Attributional Ambiguity Analysis.” Journal of Personality and Social Psychology
37

: 2297–2306.

12

Vasilescu, Bogdan, Andrea Capiluppi, and Alexander Serebrenik. 2014. “Gender, Representation and

(

)

Online Participation: A Quantitative Study.” Interacting with Computers 26

: 488–511.

Williams, Wendy M., and Stephen J. Ceci. 2015. “National Hiring Experiments Reveal 2:1 Faculty
Preference for Women on STEM Tenure Track.” Proceedings of the National Academy of Sciences
112

: 5360–65.

17

Wooldridge,  Jeffrey  M.  2010.  Econometric  Analysis  of  Cross  Section  and  Panel  Data.  Cambridge,

(

)

5
(

)

MA: MIT Press.

THE AMERICAN ECONOMIC REVIEWOCTOBER 2019