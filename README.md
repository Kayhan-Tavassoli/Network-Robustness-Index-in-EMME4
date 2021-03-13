# Network-Robustness-Index-in-EMME4
It's been a while since we lost access to #EMME4 due to the US sanctions. Bitterly regretting not having appreciated open-source software (Pedro Camargo's AequilibraE in particular), I figured why not share some scripts I had written in EMME4 Notebook and keep my efforts from going vain?

This script, written in EMME4 Notebook, ranks transportation links in order of their Network Robustness Index (NRI). Employing User Equilibrium (UE) assignment model, it first assigns the traffic to the intact input network (the base scenario), then goes through the network, sequentially disrupting links and assigning the traffic. Having kept record of the delays incurred to the network with each link disrupted, it finally returns a pandas Series containing links ranked in order of their NRI value. It often generates insightful results and if lucky, one gets to come across cases of Braess's paradox by negative NRI values.
