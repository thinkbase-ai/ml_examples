# Machine Learning Examples
ThinkBase is a SaaS Knowledge Graph system. 
Using it you can create Knowledge graphs that you can use in a variety of environments.
These ThinkBase knowledge graphs are active engines, capable of inference. You can interrogate the graphs in a variety of ways, 
by seeking the conditions that satisfy a particular node in the graph, or by searching out from a particular node looking for posibilities.
In each case the KG can be interrogated interactively, via a chat type interface.

Interaction with the SaaS can be performed via a variety of methods and user interfaces, but the common denominator is a GraphQL interface, 
offering queries, mutations and subscriptions.

You can also machine learn Knowledge Graphs directly from data. In order to do so, you have to supply that data, and a description of the data items and how to extract them from the data.
Machine learning data is typically composed of a series of examples. We'll call these patterns. You can load XML, Json or CSV data containing patterns.

You can preload the data, pattern by pattern, or load an entire set of examples at training time. In each case, the system will need to know how to extract patterns, and how to find the individual data items, and what type to apply to them.

This repository contains a set of examples of pre-coded machine learning data sets and data descriptions.

They are written in the GraphQL query language, a cut-down form of Json, and can be pasted into the GraphQL plaground UI you can find at [https://darl.dev/api](https://darl.dev/api)

Although these examples all run quickly, machine learning can be time consuming. The machine learning interface is therefore provided as a GraphQL subscription. 
You start the subscription by supplying the GraphQL source, and the system notifies you when the process is complete.

These examples can simply be pasted into the GraphQL playground interface.

ThinkBases LLC is a private organisation, not funded by government grants or private donations, so in order to pay cloud fees we need to charge a small monthly fee. You will need to have set up an account and paid for the most basic subscription to try these examples and to run your own data.

## Extracting patterns.
Tree shaped data representations, like XML and Json can encode patterns in a variety of ways.  In order to extract the data, a path is required to identify each pattern, and a separate, relative path is required to locate each data item relative to the patterns. 
ThinkBase uses XPath for XML and JPath for Json to describe these paths. 
For CSV data it is assumed that each row contains a pattern, so the patternpath is not needed, and that a header is present that can be used to identify each column.
The relative paths are therefore required to match these column names.

