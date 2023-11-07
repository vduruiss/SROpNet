# SROpNet - An Operator Learning Framework for Spatiotemporal Super-Resolution of Scientific Simulations

**Authors: [Valentin Duruisseaux](https://sites.google.com/view/valduruisseaux) and Amit Chakraborty**


<br />

This repository provides animated versions of the results presented in our paper


   [**An Operator Learning Framework for Spatiotemporal Super-Resolution of Scientific Simulations.**](https://arxiv.org/abs/2311.02328)
<br />
   [Valentin Duruisseaux](https://sites.google.com/view/valduruisseaux) and Amit Chakraborty, 2023.


<br />
<hr>

# Table of Contents

*  [**1D Diffusion with Parametric Forcing**](#1d-diffusion-with-parametric-forcing)

*  [**1D Diffusion with Forcing and Varied Initial Conditions**](#1d-diffusion-with-forcing-and-varied-initial-conditions)

*  [**1D Diffusion with Parametric Forcing and Varied Sensor and Prediction Locations**](#1d-diffusion-with-parametric-forcing-and-varied-sensor-and-prediction-locations)
  
*  [**2D Diffusion with Fixed Diffusion Constant**](#2d-diffusion-with-fixed-diffusion-constant)

*  [**2D Diffusion with Varied Diffusion Constant**](#2d-diffusion-with-varied-diffusion-constant)

*  [**2D Forced Diffusion**](#2d-forced-diffusion)
 
*  [**2D Kolmogorov Flow**](#2d-kolmogorov-flow)







<br />
<br />
<hr>
<hr>

## 1D Diffusion with Parametric Forcing

Here, each data sample corresponds to a solution to a Forced 1D Diffusion equation with a different forcing term.

![Diff1D_Exp1](https://github.com/vduruiss/SROpNet/assets/81578633/aeba328e-c435-4ae7-ad8a-3f10fc2031a0)


<br />
<br />
<hr>
<hr>

## 1D Diffusion with Forcing and Varied Initial Conditions

Here, each data sample corresponds to a solution to a Forced 1D Diffusion equation with a different initial state. We learn the dynamics with different SROpNets, using different existing super-resolution approaches as part of architecture.

![Diff1D_Exp2](https://github.com/vduruiss/SROpNet/assets/81578633/0ffaf56b-5c87-4db2-a84a-af0c2a24526e)





<br />
<br />
<hr>
<hr>

## 1D Diffusion with Parametric Forcing and Varied Sensor and Prediction Locations

We now consider a dataset where each data sample corresponds to a solution to the Forced 1D Diffusion equation with a different forcing term. In addition, we sample randomly the locations of the low-resolution sensor locations and high-resolution prediction locations, as shown in the example below

![1D_Experiment3_Locations](https://github.com/vduruiss/SROpNet/assets/81578633/dedb62ae-7ae8-4479-8423-9db1aa9bc0d2)


We compare our results with those obtained using cubic interpolation

![1D_Experiment3_Results](https://github.com/vduruiss/SROpNet/assets/81578633/f902c045-fb39-469a-8a8c-6674154a820e)





<br />
<br />
<hr>
<hr>

## 2D Diffusion with Fixed Diffusion Constant

Here, every data sample corresponds to a solution to the 2D Diffusion equation with the same diffusion constant, but with different initial states

https://github.com/vduruiss/SROpNet/assets/81578633/23522000-96fc-4060-b6e5-13cbd9170855

https://github.com/vduruiss/SROpNet/assets/81578633/da5fd1c2-baa6-47d3-bc8b-e6a922df558a

https://github.com/vduruiss/SROpNet/assets/81578633/8586c554-2cd5-4aa3-b6ad-98891a1aed6b 



<br />

<br />

Here is one more example with the low-resolution numerical solution counterpart

https://github.com/vduruiss/SROpNet/assets/81578633/35790274-44b8-4519-b677-e0f7cf1c9c0d

https://github.com/vduruiss/SROpNet/assets/81578633/d1d90e51-25b3-4dba-81fb-07da6b8a1c62



<br />
<br />
<hr>
<hr>


## 2D Diffusion with Varied Diffusion Constant

Here, each data sample corresponds to a solution to the 2D Diffusion equation with a different diffusion constant and a different initial state

https://github.com/vduruiss/SROpNet/assets/81578633/c682f9b9-8351-4a20-b979-c492c46eca6f

https://github.com/vduruiss/SROpNet/assets/81578633/05f4dfbd-c086-4d90-9749-9c5d169343b5

https://github.com/vduruiss/SROpNet/assets/81578633/c5e2cfdc-b5ee-4e71-9e0a-e6a573aec3b0


<br />

<br />

We also tested our approach on diffusion dynamics with larger diffusion constants outside the interval of diffusion constants experienced during training. We compare our results against a similar operator learning architecture which only takes the high-resolution initial state and the prediction locations as inputs.

https://github.com/vduruiss/SROpNet/assets/81578633/f31566b7-515b-4509-957c-930225754e5c

https://github.com/vduruiss/SROpNet/assets/81578633/6f2acf0c-9ec5-4386-a30a-1728f5dbc7a0

https://github.com/vduruiss/SROpNet/assets/81578633/4c5992f7-825e-4d84-a07a-9554c3ca8ee3







<br />
<br />
<hr>
<hr>

## 2D Forced Diffusion

Here, each data sample corresponds to a solution to the 2D Forced Diffusion equation with a different diffusion forcing term and a different initial state

https://github.com/vduruiss/SROpNet/assets/81578633/08fc1acf-4b42-408f-b8f6-aa4cafa91918

https://github.com/vduruiss/SROpNet/assets/81578633/cc59e4c0-c4b5-4b16-b2f4-9a0456250cc3

https://github.com/vduruiss/SROpNet/assets/81578633/cc75d200-7e42-468d-9421-a193e7d817fa





<br />
<br />
<hr>
<hr>

## 2D Kolmogorov Flow

We now consider the 2D Navier-Stokes equations in vorticity form for a viscous incompressible fluid.


<br />

We first consider the case where all the data samples correspond to the same Reynolds number Re = 20, but with different initial states


https://github.com/vduruiss/SROpNet/assets/81578633/97643adc-58a9-4d90-af9b-05ad3a98a201

https://github.com/vduruiss/SROpNet/assets/81578633/9520a96c-5938-4e17-93b7-997e40afcc10

<br />

<br />

Next, we consider the same dataset but only use the first half of the low-resolution simulationas input of the branch network.


https://github.com/vduruiss/SROpNet/assets/81578633/79f62fdc-4eaa-490e-95a6-951f08d956ca

https://github.com/vduruiss/SROpNet/assets/81578633/2297840a-bc61-4f16-8884-134ccaf8bc61


<br />

<br />

Finally, we consider the case where each data samples corresponds to a different Reynolds number in [200,500] with a different initial state

https://github.com/vduruiss/SROpNet/assets/81578633/7fb671fe-7019-4dd7-b673-bc489d43702e

https://github.com/vduruiss/SROpNet/assets/81578633/6a4797a0-82e2-4eae-88c4-977fb780ad21

https://github.com/vduruiss/SROpNet/assets/81578633/ccc80b6b-27b1-497d-b0a4-1d5edcbf44a6

