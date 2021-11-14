---
layout: page
permalink: /Research Experiences/
title: Research Experiences
description: The following are research projects I worked or am working on. 
nav: true
---

* (The list will be replaced with the table of contents.)
{:toc}

***

### **Knowledge Graph for Link Prediction and Query Answering**
A knowledge base (KB) such as Wikidata and DBpedia stores statements about the world around us. By their very nature,  KGs are far from complete as the state of the world evolves constantly. This has motivated work on automatically predicting new statements based on known statements. Centraling around this motivation, we developed different methods to aid in knowledge graph completion.

<ul>
	<div class="row">
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/TransGCN.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="caption">
			Inspired by the success of graph convolutional networks (GCN) in modeling graph data, we proposed a unified GCN framework, named <a href="https://arxiv.org/pdf/1910.00702.pdf"> TransGCN </a>, to handle heterogeneous relations in KGs by  using a novel way of representing heterogeneous neighborhood between entities and relations.
		</div>
	</div>
	<div class="row">
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/time2box.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="caption">
			The world is ever-changing. Almost all statements in knowledge bases have a temporal scope during which they are valid. In order to find out missing statements as well as their temporal scopes, we established a new knowledge base embedding framework, called <a href="https://arxiv.org/pdf/1910.00702.pdf"> TIME2BOX </a>, that can deal with atemporal and temporal statements of different types simultaneously. 
		</div>
	</div>
</ul>

### **Transformer for Traffic Prediction**
Traffic forecasting is a challenging problem due to the complexity of jointly modeling spatiotemporal dependencies at different scales. Recently, several hybrid deep learning models have been developed to capture such dependencies. These approaches typically utilize Convolutional Neural Networks (CNNs) or Graph Neural Networks (GNNs) to model spatial dependency and leverage Recurrent Neural Networks (RNNs) to learn temporal dependency. However, RNNs are only able to capture sequential information in the time series, while being incapable of modeling their periodicity e.g., weekly patterns. Moreover, RNNs are difficult to parallelize, making training and prediction less efficient. In this work, we proposed a novel deep learning architecture called <b>Traffic Transformer</b> to capture the continuity and periodicity of time series and an additional GNN to model spatial dependency. 
<ul>
	<div class="row">
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/traffic_transformer.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/transformer_encoder.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="caption">
			Our work takes inspiration from Google's Transformer framework, since machine translation and traffic prediction share some structural similarities. In machine translation, the aim is to translate a source sentence written in one language into a target sentence in another language by using a sequence-to-sequence learning framework, where the source and target sequences both consist of tokens. Traffic prediction can be formulated in a similar way. We proposed Traffic Transformer and its encoder cell as shown above for dealing with time series data. More details are describled in <a href="https://onlinelibrary.wiley.com/doi/full/10.1111/tgis.12644"> our paper </a>.		
		</div>
	</div>
</ul>

### **Qualitative Spatial and Temporal Reasoning**
Qualitative spatial/temporal reasoning (QSR/QTR) play a key role in research onhuman  cognition,  e.g.,  as  it  relates  to  navigation,  as  well  as  in  work  on  roboticsand  artificial  intelligence.  Studying how to represent qualitative spatial and temporal information and how to draw inferences on top of these representations have been an ongoing research direction for decades. In an era of representation learning, I am interested in how to subsymbolically represent and reason spatial and temporal information. 
<ul>
	<div class="row">
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/quaternionE.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="caption">
			We applied embedding methods to handling noise and efficiency problems that plagued prior work for qualitative reasoning  and  inference for tasks such  as  query answering and knowledge base completion. We explored research questions: How do embedding-based methods perform empirically compared to traditional reasoning methods ? If the performance is better, what causes this performance? We proposed a hyperbolic embedding model, called HyperQuaternionE, which is capable of capturing varying properties (such as transitivity and symmetry), inversion relations, and relation compositions (i.e., composition tables). 
		</div>
	</div>
</ul>

### **Recommender System**
Recommender systems can collect information on users’ preferences for certain items or services through their online behaviours and recommend items or services that best fit their preferences. With the prevalence of mobile devices and the development of location technology, many location-based social network services have been developed in recent years, such as Foursquare and Gowalla. When people visit and check in at a place, their locations and check-in information are shared with other people via these social media. This type of check-in information can form new social interactions and help people explore places of interest. Many location-aware recommendation systems, e.g. point of interest (POI) recommendation, use these check-in data to help people find interesting places. In order to take advantage of spatial clustering phenomena and temporal patterns of users' visits to facilitate recommendation, we proposed a <a href="https://www.tandfonline.com/doi/full/10.1080/13658816.2017.1400550"> Feature-Space Separated Factorization Model (FSS-FM)</a>.

<ul>
	<div class="row">
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/poi_recommendation.jpeg title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="caption">
			We assume that each entity has multiple features: intrinsic features, which are basic information about the entity, and extrinsic features, which are introduced by its relations with other entities. Specific to POI recommendation, the matrices of user latent factors and POI latent factors contain a mixture of basic features and other information about users and POIs, such as geographical environment and temporal sequence, which constitute the extrinsic features of POIs. The users’ preferences for a certain POI are not only decided by the extrinsic feature of this POI, but also influenced by contexts. The FSS-FM model captures each feature space with a separate slice, and all features of an entity can be considered as the sum of the separate slices.
		</div>
	</div>
</ul>

### **Impact of Places of Different Types on COVID-19**
Effective policies such as lockdowns or restrictions of certain types of businesses have been popular measures to  mitigate disease transmission. Many policies regarding COVID-19 are centered around two aspects -- place types and geographic regions. For the former, recognizing high-risk place types is assumed to be the key to success. For the latter, many policies aimed at  individual geographical region and ignored the interdependence among regions, e.g., due to human movement. We investigated the regional impact of local policies concerning place types on infectious diseases and proposed an individual-based simulation framework at place type level to evaluate effects of place type-based policies and local policies across regions.
<ul>
	<div class="row">
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/placetype-based_simulation.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="caption">
			Illustration of contact network construction, which will be used for the simulation of disease transmission. We used <a href="https://github.com/ryansmcgee/seirsplus">SEIRS Network Model</a> to achieve this simulation.
		</div>
	</div>
</ul>

### **Representation Learning for Urban Zone Representation**
Being able to characterize urban zones and regions is an important prerequisite tounderstanding the structures, patterns and dynamics of urban areas. Recently, theidea of representation learning has been applied to approach this by learning a vectorspace for regions, where each zone/region is represented as a low-dimensional vector,a.k.a. zone embedding. However, most existing work has only focused on learningstaticzone embeddings. These, however, fail to reveal the spatial interaction betweenzones during different temporal contexts. For instance, there is a strong interaction(human  mobility  flow)  between  residential  areas  and  central  business  district  ar-eas during weekdays while the same zones show a low interaction on weekends. Tobridge  this  gap,  we  propose  a  time-aware  embedding  learning  framework  from  a Heterogeneous Information Network (HIN) perspective, where human mobility and geospatial semantics (e.g., place types) are organized in a directed HIN and the tem-poral dynamic between zones is considered explicitly.
<ul>
	<div class="row">
		<div class="col-sm mt-3 mt-md-0">
		    {% responsive_image path: assets/img/TimeAwareHIN.png title: "example image" class: "img-fluid rounded z-depth-1" %}
		</div>
		<div class="caption">
			We constructed a zone-zone relevance graph and a zone-zone interaction graph to consider differences of urban zones in human mobility and geospatial semantics. We experimented with real-world datasets from Manhattan, New York City to learn time-aware zone embeddings. The results demonstrated the superior performance of our zone embeddings in terms ofrecognizing urban functional zones compared with well-known baseline methods using multiple standard evaluation metrics. 
		</div>
	</div>
</ul>





