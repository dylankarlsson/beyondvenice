---
layout: post
title: Networks and Community
author: dk
date: 2019-03-17
---
<iframe src="https://public.tableau.com/views/FiguresofBeyondBaroque/Dashboard1?:showVizHome=no&:embed=true&:display_count=yes"
 width="800" height="500"></iframe>


This chart presents an alternative view of the data contained in the calendar collection. A network is a highly suggestive form. Though network graphs are a useful tool for analysis, they are not the only way to conceptualize the distribution of connections made in a community. The chart shows the weight of a person's appearance in a given range of time.


## [View the Networks](https://dylankarlsson.github.io/bb-networks/#/)


## The Process


As a part of working to organize the Beyond Baroque archival collection, Johanna Drucker and a revolving team of students took to digitally scanning non-unique materials such as event flyers, calendars, and announcements. The digital scanner was equipped with Optical Character Recognition (OCR) software that could render the mediated, archival text into machine-readable, plain text. This rendering of material text into digital is not without errors, as degradation, layout design, and typographical variation can cause for misreadings or misrenderings of the text. In order to create these networks, I focused on developing data from a set of programming calendars used throughout the years. Using the OCR event calendars, the plain text files were run through a Named Entity Recognition script that pulled out strings of text that could be identified as potential names. With considerable cleaning of this data using OpenRefine and Excel, an edge list was created with projectoR, an RStudio package written by Matthew Lincoln.


Where each appearance of a person’s name in the calendar is constitutive of a record, the edge list connects people through their co-appearance in the calendar. Effectively, each edge represents two writers, artists, or administrators’ co-appearance in this calendar. The usefulness of a calendar in form as a temporally-bound document, allows for each connection represent involvement in the same ecosystem at the same time. While this, conceptually, is not as clear as defining relationships based on particular workshops or events, it still provides an aggregate view of the literary community's change and evolution throughout its decades of existence. Based on the scope of this project, event-based edges will be developed in future iterations with better access to Regular Expressions. Here, the edges are weighted, with higher weight visually represented by a more solid gray line, with lower weighted edges represented by a more transparent, lighter-shaded line. If viewing the networks within the Network viewer above, it is recommended to select the "purple-transparent2" style, as it was designed particularly for these networks.


## A Note on Absences in Data


The data used in this project is impacted by the preservation and digitization of archival materials, as well as the “cleanliness” of the OCR reading function. OCR is an imperfect process that can often misread and misrender text. Sometimes in creative ways, other times, in truly unhelpful ways. OCR readings can be affected by scan quality, material condition, typographical clarity and standardization, and layout design among other factors. Beyond Baroque's programming calendars are visually artistic documents in their own right. Typographical features are a large part of the artistic production of the organization. OCR can struggle with reading certain typesets and document layouts, which did have an effect on the reading of certain calendars. Absences can be compounded with each computational iteration, so it is important to be aware of how data is elided or obscured in these processes. At each level some data is lost, from OCR scanning, to text conversion, to Named Entity Recognition, and data cleaning. Mindful of these absences, and the absences already present in Beyond Baroque's calendars, I proceed with full intention of knowing the archive and the network cannot hope to capture an exact image of what was.


## The 1960s and 70s


The period ranging from 1968 to 1979 was a time of growth and creation for Beyond Baroque, as George Drury Smith’s shopfront was turned from office to literary hub. Wednesday night readings regularly brought poets and artists to the location on Washington Boulevard. The network here shows a tight nit group centralized mostly around the founder George Drury Smith. His degree centrality shows how ever-present he was in the early days, as both founder and central administrator. Jack Hirschman and Madison Morrison also have a central presence in the network as poets who were actively being published in the scene. Alexandra Garrett is also a key figure with a high eigenvector centrality, as she is connected to Smith, Hirschman and Morrison. She first met Smith in 1973 at a conference in San Diego called the Committee of Small Magazine Editors and Publishers (COSMEP), and soon became the administrator in charge of Beyond Baroque’s Library of Independent Press Literary Publications. Her value to the foundation was not unrecognized, as she later became the vice president in 1979.

[![1960s and 70s](https://i.postimg.cc/BnPcmCbn/60-70onemode-weight-csv.png)](https://postimg.cc/gxdZJ83C)


## The 1980s


Starting in 1979, the new location of the Old Venice City Hall gave the foundation an established space for readings, performances, and gallery shows. With the growth of event programming and the incorporation of the NewComp Graphics Center, a new production and publishing facility, the 1980s saw an increase in the size of Beyond Baroque’s network of distribution. The central clustering of nodes in this network shows a higher weight of a person’s presence throughout the 1980s, whereas smaller weight and location on the periphery may show sparse entry into the community. Certain figures have high betweenness centrality in this network, existing on the outskirts of the central cluster, including figures like Ron Koertge, Benjamin Weissman and Bob Flanagan, all who were integral to the literary community in Los Angeles.

[![1980s](https://i.postimg.cc/9f3PKqwt/80onemode-weight-csv.png)](https://postimg.cc/Hr277n2V)


## The 1990s


After the financial struggles of the 1980s, Beyond Baroque saw a drastic growth in the number of connections between literary communities in Los Angeles. Despite this outgrowth of connections and a renewed vitality in the programming as a result of Fred Dewey’s early leadership as director of Beyond Baroque, the literary scene was in a sense more dispersed and fragmented. The network has a central clustering of nodes with several key figures with high degree centralities like Benjamin Weissman, Luis Alfaro, and Richard Grossman. Although these were important presences in Beyond Baroque, there were many other small outgroups who were just beginning to form relationships with Beyond Baroque, such as Harryette Mullen who was just entering the Los Angeles poetry scene in the nineties. Other scenes were also starting to be featured in Beyond Baroque programming, as poets from other cities visited to give readings, such as Camille Roy and Kevin Killian.

[![1990s](https://i.postimg.cc/QxCh7G9R/90onemode-weight-csv.png)](https://postimg.cc/z3ssmQkj)


## The 2000s


The 2000s was ushered in by the leadership of Fred Dewey, who is centrally located in this network. Despite the continuing growth of output in programming, Beyond Baroque again fell into struggles over their control of the property. Higher weighted connections are present in this network, meaning that each edge represents a deeper connection, i.e. more co-appearances. While there are changes to the scene, it is becoming more fully-fledged and perhaps more contained, as people appear more, more times. Key figures in this network include Nancy Agabian, who has a high betweenness centrality as a high-weighted interlocutor between many nodes. Agabian began writing poetry in Michele T. Clinton’s poetry workshop at Beyond Baroque in the nineties, and eventually became an artist-in-residence for five years. One of the many connections Nancy Agabian has is with George Drury Smith. Smith is still connected to the community, though centrality has shifted towards more active administrators and community members. His work in building the foundation has provided a venue for this ecosystem, and the dynamic relationships that exist within it.

[![2000s](https://i.postimg.cc/wBXpz9Zs/00onemode-weight-csv.png)](https://postimg.cc/zLGMSYJJ)
