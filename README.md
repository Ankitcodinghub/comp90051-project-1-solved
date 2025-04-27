# comp90051-project-1-solved
**TO GET THIS SOLUTION VISIT:** [COMP90051 Project 1 Solved](https://www.ankitcodinghub.com/product/comp90051-project-1-specification-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;120107&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP90051 Project 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Competition link: https://www.kaggle.com/t/bc342ccd41ee49f3a9256fe359c8f6d1

1 Overview

Pairwise relationships are prevalent in real life. For example, friendships between people, communication links between computers and pairwise similarity of images. Networks provide a way to represent a group of relationships. The entities in question are represented as network nodes and the pairwise relations as edges.

Furthermore, we might want to predict if an edge will form between two nodes in the future. For example, in disease transmission networks, if health authorities determine a high likelihood of a transmission edge forming between an infected and uninfected person, then the authorities might wish to vaccinate the uninfected person.

In this way, being able to predict and correct for missing edges is an important task.

Your task:

In this project, you will be learning from a training network and trying to predict whether edges exist among test node pairs.

The testing network captures new co-authorships that have arisen more recently, i.e., subsequent to the time when the training graph was constructed. The test data is a list of 2000 undirected edges, and your task is to predict if each of those test edges are really part of the authorship network or if they are fake. Half of the test edges are real, while the other half do not actually exist. Note that test edges are supplied as undirected edges, that is, they comprise a pair of authors, which differs from the training graph format, which is in the form of hyperedges. You must predict whether these test pair of authors will coauthor at least one paper together in the ‘future’, potentially in collaboration with other authors.

To make the project fun, we will run it as a Kaggle in-class competition. Your assessment will be partially based on your final ranking in the privately-held competition, partially based on your absolute performance and partially based on your report.

2 Data Format

All data will be available in raw text. The training graph data is given in a hyperedge list format, where each row represents a paper (undirected hyperedge) as a sorted list of two or more author ids. For example:

1 4 14

25 25

Figure 1: Network diagram for the hypergraph example. Authors are nodes, and on left, each paper is a hyper edge. An alternative (simpler) graph representation for the network is shown on the right, where each edge means that at least one paper exists which includes the two incident authors as co-authors.

1 2 3

3 4 5

2 5

The test edge set is in a comma separated edge list format, where each represents an edge (source node, target node). Given this 2,000-row edge list, your implemented algorithm should take the test list in and return a 2,001 row CSV file that has a) in the first row, the string “Id,Predicted”; b) in all subsequent rows, a consecutive integer ID a comma then a float in the range [0,1]. These floats are your “guesses” or predictions as to whether the corresponding test edge is from the academic co-authorship network or not. Higher predictions correspond to being more confident that the edge is real.

For example, given the test edge set of {(3,1),(3,4)} as represented in CSV format by

Id,Source,Sink

1,3,1

2,3,4

if your prediction probabilities are 0.1 for edge (3,1), 0.99 for edge (3,4), then your output file should be:

Id,Predicted

1,0.1

2,0.99

Students should not augment the project data with external data such as further academic co-authorship data.

3 Student Groups

You are expected to work in groups of 3 students. We will mark all teams based on our expectations of what a typical team could achieve: you might consider roles such as researcher, feature engineering, learning, workflows/scripting, experimentation, ensembling of team models, generating validation data, etc. and divide your identified roles among your team. You can either find team mates yourself, we can randomly assign team mates, or both (e.g. 2 with 1).

Expected Group Behaviour. We expect all students to contribute equally to their groups, to be communicative, and at all times respectful of fellow students. Your peers will be your future professional networks and possibly co-workers. Group work is an important feature of all professional machine learning workplaces, and a key generic skill developed by this project. As described below, we require submission of recorded ‘Meeting Minutes’ for at least 3 group meetings held during the course of the project. These measures promote positive group dynamics with transparency around group expectations. From past experience of classes of this size, we expect at most a tiny handful of groups to have issues working together.

4 Submissions &amp; Important Deadlines

• PDF final report (see see Section 5 for requirements) submitted through your Canvas group.

5 Report Requirements

Your final report should provide the following sections:

1. A brief description of the problem and introduction of any notation that you adopt in the report.

2. Description of your final approach(s) to link prediction, the motivation and reasoning behind it, and why you think it performed well/not well in the competition.

Your description of the algorithm should be clear and concise. You should write it at a level that a postgraduate student can read and understand without difficulty. If you use any existing algorithms, please do not rewrite the complete description, but provide a summary that shows your understanding and references to the relevant literature (remember to include citations when referencing others’ work, you are free to choose a citation format). In the report, we will be interested in seeing evidence of your thought processes and reasoning for choosing one algorithm over another.

Dedicate space to describing the features you used and tried, any interesting details about software setup or your experimental pipeline, and any problems you encountered and what you learned. In many cases these issues are at least as important as the learning algorithm, if not more important.

Report format rules. The report should be submitted as a PDF, and be no more than three single-column A4 pages. The font size should be 11pt or above. If a report is longer than three pages in length, we will only read and assess the report up to page three and ignore further pages. References do not count towards the page limit, that is, they can spill over onto the 4th page. (Don’t waste space on cover pages.)

6 Assessment

Based on our experimentation with the project task, we expect that all reasonable efforts at the project will achieve a passing grade or higher.

Kaggle Competition (13/25):

Your final mark for the Kaggle competition is based on your rank in that competition. Assuming N teams of enrolled students compete, there are no ties and you come in at R place (e.g. first place is 1, last is N) with an AUC of A ∈ [0,1] then your mark is calculated as

.

The rank-based term encourages healthy competition and discourages collusion. The other AUC-based term

– rewards teams who don’t place in the top but none-the-less achieve good absolute results.

Note that invalid submissions will come last and will attract a mark of 0 for this part, so please ensure your output conforms to the specified requirements.

Report (12/25):

The below marking rubric outlines the criteria that will be used to mark your report.

Critical Analysis Report Clarity and Structure

Final approach is well motivated and its advantages/disadvantages clearly discussed; thorough and insightful analysis of why the final approach works/not work for provided training data; insightful discussion and analysis of other approaches and why they were not used Very clear and accessible description of all that has been done, a postgraduate student can pick up the report and read with no difficulty.

Final approach is reasonably motivated and its advantages/disadvantages somewhat discussed; good analysis of why the final approach works/not work for provided training data; some discussion and analysis of other approaches and why they were not used Clear description for the most part, with some minor deficiencies/loose ends.

Final approach is somewhat motivated and its advantages/disadvantages are discussed; limited analysis of why the final approach works/not work for provided training data; limited discussion and analysis of other approaches and why they were not used Generally clear description, but there are notable gaps and/or unclear sections.

Final approach is marginally motivated and its advantages/disadvantages are discussed; little analysis of why the final approach works/not work for provided training data; little or no discussion and analysis of other approaches and why they were not used The report is unclear on the whole and the reader has to work hard to discern what has been done.

Final approach is barely or not motivated and its advantages/disadvantages are not discussed; no analysis of why the final approach works/not work for provided training data; little or no discussion and analysis of other approaches and why they were not used The report completely lacks structure, omits all key references and is barely understandable.
