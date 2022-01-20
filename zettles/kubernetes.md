# Day 5 - Kubernetes Exploration
> This zettle focusses on kubernetes, what they do, how they do it, and why does it matter It has therefore been aptly titled:

It is important to note what the heirarchy of this technology is before we jump into individual technical details. A general flow could be stated as the following:

> <- Containers -> <- Containers -> <-- Containers -->
>
> <------ Containers ------> <------ Containers ------>
> 
> ===================================
>
> <----------------- Kubernetes ------------------->

Kubernetes literally translates (from greek) to "*helmsman*" which means the steerer of a ship. Kubernetes is often referred to as the modern operating system with each container called as an application running on it.

***You should read more about it in detail whenever you get the first opportunity at the link below.***

Technically, Kubernetes has been described below via the [website](https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/#:~:text=Kubernetes%20is%20a%20portable%2C%20extensible,both%20declarative%20configuration%20and%20automation.&text=rapidly%20growing%20ecosystem.-,Kubernetes%20services%2C%20support%2C%20and%20tools%20are%20widely%20available.,Greek%2C%20meaning%20helmsman%20or%20pilot.):

> Kubernetes is a portable, extensible, open-source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation. It has a large, rapidly growing ecosystem. Kubernetes services, support, and tools are widely available.

> The name Kubernetes originates from Greek, meaning helmsman or pilot. K8s as an abbreviation results from counting the eight letters between the "K" and the "s". Google open-sourced the Kubernetes project in 2014. Kubernetes combines over 15 years of Google's experience running production workloads at scale with best-of-breed ideas and practices from the community.