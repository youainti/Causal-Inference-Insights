# What is causality?
It is rather easy to understand causality at a basic level and rather hard to establish a rigorous definition.

 - Basic definition: Causality is is the study of X causes Y
 - Rigorous definition: What does it mean to cause?
 
I'm going to take a similar approach to E.T. Jeyens and go through a set of properties that seem to make sense. 
That should let us define what we want.
I'll start with a story to motivate the properites.

## Hurricanes vs rot

Consider the following story:

1. You have a beachfront house on stilts.
2. These stilts are slowly rotting.
3. Your neighbor has a house in a similar situation.
4. A hurricane hits the beach your house is on.
5. Your house collapses, but your neighbor's does not.

What caused the houses to/to not collapse? The hurricane or the mold?

## Properties

### Probabalistic effects

We can use probability to describe how $X$ changes the probability of $Y$ occurring.
This allows us to handle non-one-to-one effects and when there are multiple causes.

### Time Structure

We want our description to avoid the case where we believe the collapse caused the hurricane or rot. 
We want the cause to follow the effect in time.

We also want a way to discuss "jointly determined" effects, so we'll allow causes to have up to the same time as the effect, i.e.

$$
t_\text{cause} \leq t_\text{effect}
$$

Although we'll have to take special care with the jointly determined effects.

### Manipulation

There is a phrase "No causation without manipulation".

Finally, we want to define causation in relation to manipulation.
For example, the "effect of rot" compares the probability of collapse with and without rot.
We conceptualize this using *theoretical* manipulations.

## Definition

We will discuss causality in terms of **causal effects**.

Causal effects are the changes in probability (or derived measures/moments) of events  conditional on the manipulation of prior (or concurrent) events (i.e. causes).


### Corollaries

#### Causation implies association (e.g. correlation)

If $X$ causes $Y$, i.e. $X$ has a causal effect on $Y$, then 
$\text{Pr}(Y|X) \neq \text{Pr}(Y)$ (CHECK AND REFINE THIS STATEMENT)

##### Association (e.g. correlation) does not imply causation

INCLUDE COUNTEREXAMPLE?

### Examples of causal statements

Standard causal and counterfactual statements.

## Estimation

So, how do we measure causal effects? That is what we care about.

Figuring out how to measure causal effects is called causal inference.
When a procedure allows one to measure causal effects, it is causally identified.

The corollaries above have a very important implication in that probability alone does not contain enough information to identify causal effects. Some other source of information must occur. These consist of the assumptions that you make and information you have about the causal mechanism of interest.

## Plan to teach causal identification/inference

1. Pearl's Do calculus
	- Time and influence structure gives us identification.
    - Types of questions to ask 
    	- generic causal vs counterfactual
        - Direct effects vs Total effects
1. Structural Estimation
	- Incorporating functional information (monotonicity etc).
    - Dynamic Models etc.
1. Potential Outcomes Framework
	- Randomization, good as random, 
    - use of implicit structural models.
    - Threats to validity
