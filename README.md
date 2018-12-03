# CFD-in-TensorFlow

## Work in progress

The goal is to apply TensorFlow capabilities to train a network on Fluid Dynamics data.

Current dataset shown below, contains velocity magnitude for flow in a microchannel with random obstacles:

![alt text](/img/1.png)

![alt text](/img/2.png)


## data shape
Obtaning CFD data is not an easy task, especially having random objects makes the process more complicated. This is since the domain needs to be meshed and things become complicated from the aspect of how and where data points are collected.

Here, the mesh has been fixed as a remedy, limiting the problems that can be handeled. The data therefore consitis of a velcosity magnitudes on an array of 50x100 domain. The first 50 mark the inlet, and therefore, their velocity magnitude is identical to inlet velocity of the problem. The rest are calculated velcosity magnitudes influenced by existance of randomm objects. The place of objects is marked by NaN data points (or perhaps zero velocity magnitudes).
