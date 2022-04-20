# Priority coding

* There has to be priority coding since we don't process all the information
* These priority coding methods are diverse, operate at different timescales (10ms - months ??)
* The number of priority coding neural mechanisms have been small -- small number of mechanisms might underlie broad range of behaviours? 

## Forms of priority signatures

What should be considered different types of prioritization and what as the same? 

**Perceptual learning, goal-directed visual attention, salience**

* Perceptual learning
* Goal-directed attention filters out task irrelevant (but not task relevant) information?
* Visual saliency
	* Pop-out visual saliency
	* Gradation of it using (what was this one)
	* Magnitude codes
	* Gaze-based measures of visual saliency

**Higher-order object-based priority processes**

* Image memorability
* Novelty

**Talk about (six) different neural prioritization mechanisms here**

* How to separate behaviours and neural measurements that are correlated (but not causal) compared to *true* priority coding mechanisms (causal)? 
	* Rather than studies that say "When behavioural X decreased, neural Y decreased as well", there should be a more *parametric* variation of stimulus and concomitant modulation should be seen neural mechanism (Parker and Newsome, 1998) -- this is more powerful
	* Evidence for a "readout change" mechanism in LIP while studying perceptual learning in a motion detection task ? (Josh Gold 2008 Nat Neuro)
		* Another showing V4 noise correlations go down with perceptual learning? 
		* Changes in noise correlations could cause changes in the way inputs from visual cortex are *read out* by association areas (why is this interesting?). Are they saying that the private subspace changes - changing the communication subspace dimensionality - leading to a different readout? 

**A unified but distinguishable(?) code**

*INSIGHT 1*
* Population activity (being used) exists in a lower dimensional subspace (lower than the actual dimensionality)
	* Attention seems to modulate activity in low-dimensional subspaces
	* In IT, mapping between novelty and neural activity is linearly decodable -- *they say this is 1 dimensional?* (why does this imply low-dimensionality?!)
		* It doesn't! I can have 2 3-dimensional point clouds which can be linearly separable! Wtf. 

*INSIGHT 2*
* Subspace in which priority is associated with response modulations seems to be such that it doesn't affect the identity
* This is also in line with magnitude coding hypotheses where priority coding multiplicatively scales but doesn't change representation -- but here the sensitivity will increase with the scaling, thus affecting behaviour
* The subspace intuition gives a way to interpret behavioural modulations which are observed even when there is not a large change in the population response as a result of priority coding 
	* A communication subspace idea suggests that the activity modulation in dimensions aligned with behaviourally relevant variables should affect behaviour


*INSIGHT 3*
* Different forms of prioritization affect partially overlapping subspaces of activity (not super orthogonal?)
	* Since different forms of prioritization affect the grand mean firing rate they imply some correlation with the magnitude dimension
	* This means that from the magnitude, we can read out that some (or many) priority codes are active. But how does the brain separate those? 
		* Although these codes have some projection on the magnitude coding axis, they are inherently low dim, that is, they are only weakly correlated with each other -- This allows the brain to separate these different priority codes? 

*INSIGHT 4* 
* Communication between areas can be made better *without* changing the communication subspace dimensionality but just by increasing fidelity within the communication subspace
	* They refer to ruff and cohen study where shifting attention between opposite hemifields has negligible effects on the representation (amount of information and subspace) but changes the representations (rather than the decoding strategy!)
	* How does the changing of alignment in communication subspaces look like in the population activity?

* Priority coding has a unified code (in the sense of magnitude coding) but also separate from each other since different priority codes are only partially overlapping

## Future directions 

* Could help constrain network model assumptions (make the communication subspace low-dimensional). But model networks can't perform tasks for which prioritization is necessary?
* DANNs - another class of models used to understand representations in the brain (different layers correlate with different areas' representations)
	* Memorability coding emerges from these networks -- Layer correlated with IT responds highly to some objects and these objects' memorability high in humans
	* Strength 1 - They can be used to explain single neuron (or population) responses to complex stimuli
	* Strength 2 - They help us understand nuisance variation (variation along dimensions not relevant to task) - help us understand transformation along the ventral stream (from highly non-linear to linear formats in later areas)
	* Drawback -> They lack trial-to-trial variability
* In a model, we can achieve prioritization by modulating populations response (small EI ratio changes)
	* This trickles to downstream areas and since these are multiplicative, identity is not affected
	* But do these support the neural correlates of priority coding seen in recordings?

## How and where can we use these insights in the lab?

---
* TODO Read Marlene's Science 2018 study -- what does it say? (Cited as study showing reduction of noise correlations with learning)