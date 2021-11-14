---
layout: page
permalink: /interns/
title: Interns and Projects
description: The following are projects I have done while being an intern for companies or a research assistant.
nav: true
---

* (The list will be replaced with the table of contents.)
{:toc}

***

### **1. Intern as Machine Learning Researcher at Siemens**
In this project, I focused on knowledge graph completion and query answering by using knowledge graph embedding (KGE) methods. A common assumption in KGE is that similar entities are more likely to play similar relational roles or share similar local graph structures. However, previous works usually rely on triple-level structural information while ignoring long-term relational dependencies between entities. Inspired by Transformer in capturing long-term dependencies between words in sentences, I developed a transformer-based embedding model to capture relational dependencies for knowledge graph completion. The main difference lies in that relational roles of entities should be incorporated instead of pure entity connections (corresponding to word proximity in sentences).

### **2. Research Assistant on an NSF Project - <a href="https://www.nsf.gov/awardsearch/showAward?AWD_ID=2033521&HistoricalAwards=false"> KnowWhereGraph </a>**
The goal of this project is to improve data-driven decision making and data analytics, specifically data analytics that involve geographic data. This project will create the “KnowWhereGraph” – a knowledge graph tool that specifically enables other data-analysis knowledge tools that have a geospatial component. Two core components in our “KnowWhereGraph” are a seed knowledge graph that  contains  a  wide range of integrated datasets at the human-environment interface (e.g., soil, hydrology, humantarian relief), and a series of geospatial enrichment services on top of our graph for a  wide  range  of applications in environmental intelligence by giving decision-makers and data analysts on-demand access to area briefings. 

Mutiple research topics are involved in this project, including knowledge graph construction, ontology engeneering, event detection, causal relation identification, expert-expertise match, knowledge graph summarization, and data integration, etc. Paricularly, I am working on developing approaches to matching experts and expertise and identifying causal events by using pre-trained language models. Additionally, I also help on designing ontologies for domain datasets and help triplify those datasets into our seed graph. 

More details and demos be found on our <a href="http://www.knowwheregraph.org/">project website </a>. One example of using our services for humantarian aid is shown below (Please refer to our paper for more details.):

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
		    {% responsive_image path: assets/img/hazard.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="col-sm-4 mt-3 mt-md-0">
		    {% responsive_image path: assets/img/Expert.jpeg title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="caption">
			 The two figures show the materialization of an expert and a hazard in our expert-expertise knowledge graph, respectively. Each expert may be linked to expertise topics of various types, which are instances of kwg-ont:ExpertiseTopic. We identied expertise topics from experts' publications by using <a href="https://arxiv.org/pdf/2008.06877.pdf">TopicBert</a>. 
		</div>
</div>

<div class="row">
	<div class="col-sm mt-3 mt-md-0">
		{% responsive_image path: assets/img/follow-your-nose.png title: "example image" class: "img-fluid rounded z-depth-1" %}
	</div>
	<div class="caption">
		We designed a follow-your-nose style expert navigation tool, based on the PhuzzyLink framework to assist relief specialists who are not familiar with Semantic Web techniques (e.g., SPARQL querying)efficiently explore the expert knowledge graph. 
	</div>
</div>

<div class="row">
	<div class="col-sm mt-3 mt-md-0">
		{% responsive_image path: assets/img/dr_similarity.png title: "example image" class: "img-fluid rounded z-depth-1" %}
	</div>
	<div class="caption">
		The figure on the left shows an example of searching result. When a usertypes “Bryan Grenfell”, this interface will guess possible experts who are similar to the user’s input. We measured the similarirty by their publications using <a href="https://cs.stanford.edu/~quocle/paragraph_vector.pdf">Doc2Vec</a>. 
	</div>
</div>

### **3. Research Assistant on an NSF Rapid Grant**
In this project, we focused on studying the ever-changing role of different places in spreading COVID-19. During the recent COVID-19 pandemic, many coronavirus-related complications have shown to be tied to super-spreader individuals and super-spreader events such as the October convo-cation events at Charlotte church and the February conference by the drug company Biogen. Those examples reveal that virus transmission is more  ikely to happen at places of certain  types (e.g.,  churchesand  bars)  than  others.  Therefore,  identifying  super-spreading places is crucial to the government and policymakers,  so  that  place/place  type-centric policies can be enacted effectively. 

We designed an index to quantify the risk of different place types, which considers three basic features of a place – visit frequency, area, and duration  of visiting. Moreover, humans are mobile and the risk of places are directional. Residents  may  travel  to high-risk places in other counties and bring the virus back to their home counties, thus resulting in cross-region virus transmission. This implies that the total risk in a county may not only be determined by people’s visit to high-risk places in their home county but may also be largely influenced by visiting high-risk places outside. We are interested in the following questions: Q1:which  types of  places  have  more  external  influence/risk? Q2:which  counties  are  affected  more  by places outside? and Q3:which counties influence other counties more?

<div class="row">
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/external_by_sector.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="caption">
			Externality ratio by place type. Externality ratio measures the impact of places of different types on other regions beyond residing regions of places. 
		</div>
</div>

<div class="row">
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/map_external_influence.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/map_external_influencedby.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="caption">
			(a) Counties which receive more external risk. People traveling from their home counties take risk to their desitination regions. The darker shows recieving more risk from the outside.(b) Counties which transmit more risk to the outside. Places in each county pose threat to other counties. People traveling from other counties bring back risk to their home regions. The darker shows more threat to other regions.
		</div>
</div>

Four risk flow maps across the US in terms of different place types. Counties are represented as nodes and the size of anode is determined by the total risk of a county, and the risk transmitted from one county to another is represented by edges with thewidth of edge representing the amount of risk.

<div class="row">
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/amusement.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/gambling.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="caption">
			Left: Amusement Parks. Right: Gambling Locations. For Amusement parks, two significant hot-spots are observed in Orange county, Florida and Orange county, California. They have a high externality ratio and attract visitors across the US, thus spreading their risk to the entire country. Similar observations are shown in Gambling Locations.
		</div>
</div>

<div class="row">
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/bars.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/grocery.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="caption">
			Left: Bars. Right: Grocery. Differing from the above, hot spots of Bars and nightclubs, and Grocery stores are distributed across almost all counties and are strongly connected with neighboring counties. It indicates that their risk mostly circulates within a county and around their neighboring counties.
		</div>
</div>

### **4. Research Assistant on an NSF Project - Open knowledge Network**
Knowledge graphs consist of interlinked pieces of information about our world. Everything happens somewhere and at some time and knowing where and when things happen is critical to understanding why and how they happen. This project focuses on using space and time as nexuses to connect data across different domains, multimedia formats, and perspectives by using knowledge graph technologies. The resulting knowledge graph enables users to ask complicated domain questions and arrives at a more holistic understanding of complex physical and social processes. We developed text-based and image-based enrichment tools to enrich news articles and images with open knowledge graph (such as Wikidata).
<div class="row">
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/text-enrichment.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/image-geoenrich.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="caption">
			Illustration of Text-enrichment tool and Image-enrichment tool. On the left, starting with a text, we first identified places mentioned in the content and then used them to link to Wikidata to request more information about those places. On the right, starting with an imagery about a geographic region, we enriched this image by requesting events or disasters happening in this area from Wikidata. By such enrichment, users are provided with abundant information about places of their interest. This idea benifits from the wide availablity of open knowledge graphs.
		</div>
</div>




