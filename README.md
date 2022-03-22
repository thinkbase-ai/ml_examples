# Machine Learning Examples
ThinkBase is a SaaS Knowledge Graph system. 
Using it you can create Knowledge graphs that you can use in a variety of envirionments.
These ThinkBase knowledge graphs are active engines, capable of inference. You can interrogate the graphs in a variety of ways, 
by seeking the conditions that satisfy a particular node in the graph, or by searching out from a particular node looking for posibilities.
In each case the KG can be interrogated interactively, via a chat type interface.

Interaction with the SaaS can be performed via a variety of methods and user interfaces, but the common denominator is a GraphQL interface, 
offering queries, mutations and subscriptions.

You can also machine learn Knowledge Graphs directly from data. In order to do so, you have to supply that data, and a description of the data items and how to extract them from the data.
Machine learning data is typically composed of a series of examples. We'll call these patterns. You can load XML, Json or CSV data.

You can preload the data, pattern by pattern, or load an entire set of examples at training time. In each case, the system will need to know how to extract patterns, and how to find the individual data items, and what type to apply to them.

This repository contains a set of examples of pre-coded machine learning data sets and data descriptions.
They are written in the GraphQL query language, a cut-down form of Json, and can be pasted into the GraphQL plaground UI you can find at https://darl.dev/api

Although these examples all run quickly, machine learning can be time consuming. The machine learning interface is therefore provided as a GraphQL subscription. 
You start the subscription by supplying the graphQL source, and the system notifies you when the process is complete.
