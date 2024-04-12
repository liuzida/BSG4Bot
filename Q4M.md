**Q4M**: Difference from BotMoe

**R**: BotMoE observes that bot characteristics greatly vary from one user community to another. Thus, BotMoE divides all users into $n$ communities, with each community processed by an expert. Every user is assigned to the $top-k$ most likely communities. The decisions of experts are combined vis a gating network, allowing the model to adjust to different user distributions within different communities.

BSG4Bot takes one uniform biased subgraphs construction method, but may produce different subgraphs with diverse forms. As both community and subgraph provide a context for a given node, we can view the subgraphs as the communities. Thus, BSG4Bot actually train one GNN model across a large number of diverse-formed homophily communities, which may enable BSG4Bot to have more generalization than BotMoE. We guess that it is a reason that BSG4Bot outperforms BotMoE over all three datasets.
