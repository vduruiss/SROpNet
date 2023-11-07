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

![Diff1D_Exp1](https://github.com/vduruiss/SROpNet/blob/main/1D_Diffusion_Varied_Forcing/Diff1D_Exp1.png)

1D_Diffusion_Varied_Forcing/Diff1D_Exp1.png

<br />
<br />
<hr>
<hr>

## 1D Diffusion with Forcing and Varied Initial Conditions

Here, each data sample corresponds to a solution to a Forced 1D Diffusion equation with a different initial state. We learn the dynamics with different SROpNets, using different existing super-resolution approaches as part of architecture.

![Diff1D_Exp2](https://github.com/vduruiss/SROpNet/blob/main/1D_Diffusion_Varied_ICs/Diff1D_Exp2.png)





<br />
<br />
<hr>
<hr>

## 1D Diffusion with Parametric Forcing and Varied Sensor and Prediction Locations

We now consider a dataset where each data sample corresponds to a solution to the Forced 1D Diffusion equation with a different forcing term. In addition, we sample randomly the locations of the low-resolution sensor locations and high-resolution prediction locations, as shown in the example below

![1D_Experiment3_Locations](https://github.com/vduruiss/SROpNet/blob/main/1D_Diffusion_Varied_Locations/1D_Experiment3_Locations.png)


We compare our results with those obtained using cubic interpolation

![1D_Experiment3_Results](https://github.com/vduruiss/SROpNet/blob/main/1D_Diffusion_Varied_Locations/1D_Experiment3_Results.png)





<br />
<br />
<hr>
<hr>

## 2D Diffusion with Fixed Diffusion Constant

Here, every data sample corresponds to a solution to the 2D Diffusion equation with the same diffusion constant, but with different initial states

[Diffusion2D_Exp1_1](https://github.com/vduruiss/SROpNet/blob/main/2D_Diffusion_Fixed_Diff_Const/Diffusion2D_Exp1_1.mp4)

[Diffusion2D_Exp1_2](https://github.com/vduruiss/SROpNet/blob/main/2D_Diffusion_Fixed_Diff_Const/Diffusion2D_Exp1_2.mp4)

[Diffusion2D_Exp1_3](https://github.com/vduruiss/SROpNet/blob/main/2D_Diffusion_Fixed_Diff_Const/Diffusion2D_Exp1_3.mp4)

<br />

<br />

Here is one more example with the low-resolution numerical solution counterpart

[Diffusion2D_Exp1_4_LR](https://github.com/vduruiss/SROpNet/blob/main/2D_Diffusion_Fixed_Diff_Const/Diffusion2D_Exp1_4_LR.mp4)

[Diffusion2D_Exp1_4](https://github.com/vduruiss/SROpNet/blob/main/2D_Diffusion_Fixed_Diff_Const/Diffusion2D_Exp1_4.mp4)


<br />
<br />
<hr>
<hr>


## 2D Diffusion with Varied Diffusion Constant

Here, each data sample corresponds to a solution to the 2D Diffusion equation with a different diffusion constant and a different initial state

[Diffusion2D_Speeds_1](https://github.com/vduruiss/SROpNet/blob/main/2D_Diffusion_Varied_Diff_Const/Diffusion2D_Speeds_1.mp4)

[Diffusion2D_Speeds_2](https://github.com/vduruiss/SROpNet/blob/main/2D_Diffusion_Varied_Diff_Const/Diffusion2D_Speeds_2.mp4)

[Diffusion2D_Speeds_3](https://github.com/vduruiss/SROpNet/blob/main/2D_Diffusion_Varied_Diff_Const/Diffusion2D_Speeds_3.mp4)



<br />

<br />

We also tested our approach on diffusion dynamics with larger diffusion constants outside the interval of diffusion constants experienced during training. We compare our results against a similar operator learning architecture which only takes the high-resolution initial state and the prediction locations as inputs.

[Diffusion2D_Speeds_Compare_1](https://github.com/vduruiss/SROpNet/blob/main/2D_Diffusion_Varied_Diff_Const/Diffusion2D_Speeds_Compare_1.mp4)

[Diffusion2D_Speeds_Compare_2](https://github.com/vduruiss/SROpNet/blob/main/2D_Diffusion_Varied_Diff_Const/Diffusion2D_Speeds_Compare_2.mp4)

[Diffusion2D_Speeds_Compare_3](https://github.com/vduruiss/SROpNet/blob/main/2D_Diffusion_Varied_Diff_Const/Diffusion2D_Speeds_Compare_3.mp4)


<br />
<br />
<hr>
<hr>

## 2D Forced Diffusion

Here, each data sample corresponds to a solution to the 2D Forced Diffusion equation with a different diffusion forcing term and a different initial state

[ForcedDiffusion2D_1](https://github.com/vduruiss/SROpNet/blob/main/2D_Forced_Diffusion/ForcedDiffusion2D_1.mp4)

[ForcedDiffusion2D_2](https://github.com/vduruiss/SROpNet/blob/main/2D_Forced_Diffusion/ForcedDiffusion2D_2.mp4)

[ForcedDiffusion2D_3](https://github.com/vduruiss/SROpNet/blob/main/2D_Forced_Diffusion/ForcedDiffusion2D_3.mp4)



<br />
<br />
<hr>
<hr>

## 2D Kolmogorov Flow

We now consider the 2D Navier-Stokes equations in vorticity form for a viscous incompressible fluid.


<br />

We first consider the case where all the data samples correspond to the same Reynolds number Re = 20, but with different initial states

[Kolmogorov_Re20_Ex1](https://github.com/vduruiss/SROpNet/blob/main/2D_Kolmogorov_Flow/Kolmogorov_Re20_Ex1.mp4)

[Kolmogorov_Re20_Ex2](https://github.com/vduruiss/SROpNet/blob/main/2D_Kolmogorov_Flow/Kolmogorov_Re20_Ex2.mp4)


<br />

<br />

Next, we consider the same dataset but only use the first half of the low-resolution simulationas input of the branch network.


[Kolmogorov_Re20_Partial_Ex1](https://github.com/vduruiss/SROpNet/blob/main/2D_Kolmogorov_Flow/Kolmogorov_Re20_Partial_Ex1.mp4)

[Kolmogorov_Re20_Partial_Ex2](https://github.com/vduruiss/SROpNet/blob/main/2D_Kolmogorov_Flow/Kolmogorov_Re20_Partial_Ex2.mp4)


<br />

<br />

Finally, we consider the case where each data samples corresponds to a different Reynolds number in [200,500] with a different initial state

[Kolmogorov_MixedRe_Ex1](https://github.com/vduruiss/SROpNet/blob/main/2D_Kolmogorov_Flow/Kolmogorov_MixedRe_Ex1.mp4)

[Kolmogorov_MixedRe_Ex2](https://github.com/vduruiss/SROpNet/blob/main/2D_Kolmogorov_Flow/Kolmogorov_MixedRe_Ex2.mp4)

[Kolmogorov_MixedRe_Ex3](https://github.com/vduruiss/SROpNet/blob/main/2D_Kolmogorov_Flow/Kolmogorov_MixedRe_Ex3.mp4)
