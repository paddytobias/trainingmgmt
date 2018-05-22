@title[Introduction]


# Managing training content and delivery

<p><div align=center>Dr Paddy Tobias, eResearch Analyst</div></p>

<p><div align=center>Intersect Australia</div></p>


---
![training](assets/image/intersect_training_20180514.png)
---
## Context

- Increasing support for research data in universities |
- Still little support for research software code |
- But software management tools on the rise in research |


---
## Why manage your code?

- Improving your workflow |
- Coordinating group research |
- Scientific reproducibility |
- External engagement |
- Co-authorship opportunities |


+++

![Perkel, J 2016](assets/image/nature_toolbox_github-influence_06.10.2016_WEB.png)

READ: [Democratic databases: science on GitHub](https://gitpitch.com/paddytobias/research-software-management#/9/1)

+++
### 2000-2010 Biology journal articles
|Mention types|Count (%)|
|--|--|--|
|Cite s.w. publication|105 (37%)|
|In-text s.w. name only|90 (31%)|
|Instrument s.w.|53 (19%)|
|Cite project name or website|15 (5%)|
|Cite s.w. URL|13 (5%)|
|Cite user’s manual|6 (2%)|
|No name|4 (1%)|

<p style="text-align:center"><font size="4">*articles* = 91; *mentions* = 286</font></p>

<DIV ALIGN=CENTER><font size="4">READ: [Software in the scientific literature]("https://gitpitch.com/paddytobias/research-software-management#/9/1")</font></DIV>

Note:
* from 91 randomly selected Biology articles published between 2000-2010
* 59 had a mention of software in some form or another

+++

Things to consider:
- Approaches to code writing |
- Version control |
- Managing contributions |
- Develop documentation |
- Project management |
- Licensing |

+++

## How to manage your code?


### Git, GitHub, GitLab, Git-everything...


<img src="assets/image/git_logo.jpg" alt="Git" style="width: 370px;"/>

<img src="assets/image/github_logo2.png" alt="GitHub" style="width: 370px;"/>
<img src="assets/image/gitlab_logo.png" alt="GitHub" style="width: 180px;"/>
[More options here...](https://software.ac.uk/resources/guides/choosing-repository-your-software-project)

Note:
Alternative code repositories:
- BitBucket
- SourceForge

+++

![git lifecycle](assets/image/github_lifecycle.png)

Note:
Project mngmnt
https://github.com/paddytobias/surveying-with-qualtrics/issues
https://waffle.io/paddytobias/surveying-with-qualtrics

citation
https://github.com/paddytobias/15census_timor_dataclean
https://zenodo.org/record/826449#.Wt5zkBNL9E9

---

```
if <<CODING BY/FOR YOURSELF>>:


    then ...
```
+++

### Version control
- Set version control up as the first thing you do |
- Make regular commits |
- Meaningfully describe major commits, not every commit |
- Most repos have a two step process to safe-guard from errors |

<iframe class="stretch" data-src="https://swcarpentry.github.io/git-novice/fig/git-staging-area.svg"></iframe>

Note:

if you dont want to do this via command line, consider a number of desktop clients that talk to git repositories. E.g., GitHub Desktop

+++

### Writing your code
- Where possible look for open source code to work from |
- However, if wanting to adapt code from someone else, best not to. Write you're own and copy/paste the chunks you want |
- Have a plan for your code before you start writing. What do you want the code to achieve? |
- Draw plans before you write your code. Inputs and outputs? |
- Make comments in your code as write |

Note:
* there are formal design architectures you can follow (e.g., Unified Modelling Language), but you don't have to use/learn these. Just come up with a conceptual way to explain what you what your program.
* more so, draw these concepts before you begin coding.
* take into account your inputs and outputs. what goes into your program and what do you want to come out

---

```
else if <<COLLABORATING WITH OTHERS>>:


    then ...
```

+++
### Managing contributions
Git has many ways to manage contributions:
- only owners can make changes, but everyone else can recommend changes. i.e., "pull request" |
- each change is identified and marked with a unique id, meaning that you can rollback to previous versions |
- repos can be "forked", "branched", "cloned" and "merged", "upstream" and "downstream" |


+++
<img src="assets/image/atom_logo.png" alt="atom" style="height: 150px;" align="right"/>
### Documentation

- Create a README.md file for every project |
- Learn Markdown |
- Consider developing user guides as well (e.g., for installing, use, examples) |

TRY:[Atom](atom.io)

Note:
use Atom

+++
<img src="assets/image/waffle_logo.png" alt="waffle.io" style="height: 150px;" align="right"/>

### Issues/'To dos' register and Project management

- Consider issues ~ 'To Dos' |
- See software development as a project |
- Allow teammates or public to register issues |
- Track the resolution of these issues |

TRY:[Waffle.io](https://waffle.io)

Note:

https://waffle.io/paddytobias/research-software-management


---

```
else if <<PUBLISHING YOUR CODE>>:


    then ...
```
+++
<img src="assets/image/force11_logo.png" alt="Force11" style="width: 300px;" align="right"/>

### Software Citation Principles

* legitimate and citable research product |
* gives scholarly credit |
* citations should use unique identifiers |
* persistent unique identifiers (e.g., DOIs) |
* facilitate access to the software |
* specify the version |

Note:
1. considered a legitimate and citable product of research
2. facilitates giving scholarly credit, attribution to all contributors
3. citations should have recognised unique identifiers, machine actionable, interoperable
4. unique identifiers and metadata describing the software should persist
5. citations should facilitate access to the software and use of it
6.  citations should specify the version that was used


+++
### Software citation and licensing

<img src="assets/image/zenodo_logo.png" alt="Zenodo" style="height: 100px;"/>
<img src="assets/image/github_logo2.png" alt="GitHub" style="height: 100px;"/ align="right">

* Zenodo allows you to archive your code with them
* In turn Zenodo will issue you a Digital Object Identifier for the collection
(READ: [Making your Code Citable](https://gitpitch.com/paddytobias/research-software-management#/9/1))

![example](assets/image/example_doi.png)


+++
### Reproducible research...

![Code ocean](assets/image/code_ocean_CUP.png)(https://www.researchinformation.info/news/cambridge-university-press-partners-code-ocean)

+++
### Code Ocean

<iframe class="stretch" data-src="https://codeocean.com/"></iframe>


---

## Git vocabulary

```
git push  <REMOTENAME> <BRANCHNAME>
git clone https://github.com/<USERNAME>/<REPOSITORY>.git
git fetch <REMOTENAME>
git merge <REMOTENAME>/<branchname>
git pull <REMOTENAME> <branchname>
```
@[1](`push` to push or publish commits to your code repository)
@[2](`clone` to grab a complete copy of another user's repository)
@[3](`fetch` to retrieve new work done by other people)
@[4](`merge` combines your local changes with changes made by others)
@[5](`pull` completing both *git fetch* and *git merge* in the same command)

---

## Benefits
- Research Impact and Engagement |
  - engaging with end users |
  - tracking engagement |
- Global collaborations |
- More recognition for your work |
- Reproducible research |


---
## Where to next?

- Come to the [Version Control with Git](https://www.eventbrite.com.au/e/git-at-une-armidale-registration-45282864266) in two weeks: 12.30-4:30pm, **8 May**

+++
## Reference list

<p><font size="3">GitHub, 2016 "Making your Code Citable", https://guides.github.com/activities/citable-code/</font></p>

<p><font size="3">Howison, J, Bullard, J, "Software in the Scientific Literature: Problems with Seeing, Finding, and Using Software Mentioned in the Biology Literature", *Journal of the Assoc. for Information Science and Technology*, 67(9), 2137-2155, https://onlinelibrary.wiley.com/doi/abs/10.1002/asi.23538</font></p>

<p><font size="3">Perkel, J, "Democratic databases: science on GitHub", *Nature* 538, 127–128, October 6, 2016, doi:[10.1038/538127a](https://www.nature.com/news/democratic-databases-science-on-github-1.20719)</font></p>

<p><font size="3">Smith, AM, Katz, DS, Niemeyer, KE, FORCE11 Software Citation Working Group, 2016,  "Software citation principles", *PeerJ Computer Science*, 2(86) https://doi.org/10.7717/peerj-cs.86</font></p>

<p><font size="5">Code for this presentation: [github.com/paddytobias/research-software-management]("github.com/paddytobias/research-software-management")</font></p>
