> "In all situations, the government of Raikoth will take the normatively correct action."

# Discuss

Check out our [Google Group for Raikoth-Ethereum](https://groups.google.com/forum/#!forum/raikoth-ethereum) to chat about the project.

# Raikoth

[Scott Alexander](http://slatestarcodex.com/)'s fictional society of [Raikoth](http://slatestarcodex.com/2013/05/15/index-posts-on-raikoth/) represents a framework for governance worth exploring.

The [Ethereum](https://www.ethereum.org/) platform provides a number of features which may theoretically be leveraged to implement at least some parts of the Raikoth infrastructure.

This project is an attempt to implement Raikoth as an organizational entity on the Ethereum network.

# Concept

Very little of the following will make much sense without reading about the hypothetical [government of Raikoth](http://slatestarcodex.com/2013/05/06/raikoth-laws-language-and-society/). 

Try to see the concepts through the whimsical style and appreciate that Scott Alexander's goal underlying Raikoth's creation was mainly to create something novel and interesting.

In short, Raikoth's government is run on four distinct automated systems referred to as Angels:

> The Angel of Preference takes census and survey data from every citizen of Raikoth, runs it through the series of utilitarian superstructure functions ... and spits out a utility function. ... What it ends up with are a series of preference weights for possible world-states and for various subcomponents of those world-states...

> The Angel of Evidence is a system of linked “oracles” – what we would call prediction markets – heavily subsidized by the government and played not only by thousands of Raikolin but by the great financial conglomerates of Sxiro and even further afield. Fed sufficient time, money, and publicity, it can calculate the likely effects of any policy with an accuracy even the Priests of Truth cannot match...

> The Angel of Salience accepts suggestions from anyone on Raikoth... These suggestions can be any form of policy change, whether that be tax relief, new land use regulations, or the invasion of a foreign power. The thousands of suggestions it receives each day get crowdsourced, with average citizens and experts giving them upvotes or downvotes whose weight is proportional to those users’ past success rates. Eventually, the most creative or well-thought-out proposals rise to the top and become salient for further investigation.

> The Archangel ... combines input from all three Angels to render government decisions. It takes policy proposals from the Angel of Salience, uses the Angel of Evidence to estimate their likely effects, and finally runs those effects through the Angel of Preference to determine whether they would raise or lower the utility function represented therein and so bring the world closer to or further from the Divine. The set of noncontradictory policies that most satisfies the Angel of Preference becomes the law of Raikoth.

The Ethereum-based prediction market [Augur](https://github.com/AugurProject/augur) is pretty much the Angel of Evidence. A subtask of the Ethereum-Raikoth project is to determine how to most efficiently interface the DApp with Augur.

The Angel of Salience would be relatively straightforward to implement using modern web technology. The Reddit codebase seems a likely candidate framework. The validation of user accounts using the cryptographic security inherent in Ethereum should help avoid issues related to voting fraud. A decision remains regarding how ownership of the polity would be handled - e.g., one person, one vote? or votes weighted by ownership?

The Angel of Preference is probably the most difficult to specify. As outlined in the fictional Raikoth, it just sort of assumes that the problem of ethics has been reduced to a calculation. It may be feasible to start with a framework involving a detailed census of citizen preferences tied to QALY calculations, and then the inner details of the Angel of Preference can themselves be iterated on recursively until a satisfactory metaethical calculus is resolved.

Note that a good "seed" preference set will be necessary to keep the Raikoth Ethereum contract **alive** in the first place. The organization has to decide that the organization is worth funding, and has to avoid destroying or starving itself as it passes through infancy.

Note also that the same issue of polity ownership applies to the Angel of Preference. Should the Raikoth utility calculation weighted by person or by ownership share?

The part the works the least-well in real life and the most-well with Ethereum is the Archangel. Ethereum helps with the pragmatic issue of implementability here. In a sense, Archangel is just a metaphor for the interconnectivity of all the other Angels.
