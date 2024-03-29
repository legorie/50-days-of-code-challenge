# 50-days-of-code-challenge

<p>
<img src="https://raw.githubusercontent.com/legorie/50-days-of-code-challenge/master/assets/programmeur-home.webp" alt="50 Days of Code" />
</p>

[100 Days of Code Challenge](https://www.100daysofcode.com/) is an initiative I wanted to take but given my commitments are work and home, I took the liberty to divide the initial number by the number of kids I'm bless with to make it a 50 day challenge.

My goal is to learn the Go language better and contribute to an Open Souce program which I've been following since 3 months. For now, I'm not able to make heads or tails about of the K8S Operator written in Go, hopefully at the end of this #50-days-of-code-challenge it would make things better.

---

## Goals

- [ ] [Learn GoLang to a confortable extend](#)
- [ ] [Learn more about K8S Operators](#)

---
## Day 47:
25-Feb-2023
- After a suggestion from a mentoring session, I started to work on a 3 tier application written in Golang. Though the application is very simple, the different learnings on local development, using environment variables/files and implementing them on a K8S cluster was enormous. Glad I embarked on this journey :  
https://github.com/legorie/k8s-3tier-application  
For now, the sample app & deployment has the following parts :  
Step 1: Web, API and DB running on localhost  
Step 2: Dockerize the web and api applications on localhost  
Step 3: Running the application on our local Kubernetes cluster  
Step 4: Deploy in the Kubernetes cluster using a declarative YAML  
Step 5: Use Ingress controller to manage the traffic  
Step 6: Converting the deployment to a Helm chart  

## Day 46:
12-Feb-2023
- An important event in my Opensource journey, I was able to submit 2 PRs to the Kubearmor project. The PRs are still in draft state, but I had lots of learnings in writing the enhancement feature of the kubearmor-client code and the base kubearmor code.
- Running the code in my K3S environment and testing the karmor client code on my Ubuntu VM was a challenging setup which I passed more than 3 days figuring out. All in all, I can see how enriching the expreience was
- https://github.com/kubearmor/kubearmor-client/pull/254
- https://github.com/kubearmor/KubeArmor/pull/1086

![image](https://user-images.githubusercontent.com/1323423/218866375-1579eeff-99a1-493b-b408-4397dbb5977a.png)


## Day 45:
14-Jan-2023
- To keep the ball rolling on Golang, followed along and wrote a simple API application with the mux package.
- https://github.com/legorie/go-learn-projects/tree/main/go-movies-crud

## Day 44:
05-Jan-2023
- Created a simple program using K8S client-go library to list the pods in a cluster. Thanks Aditya Joshi (https://www.youtube.com/watch?v=tQvpZSWYt8E) for the simple program to iron out the basics
- Now that the program runs fine (https://github.com/legorie/k8s-client-go : first commit), I'm closing my day with more questions that I started to resolve
- I'm set out to understand & answer the following questions :  
  ❓ Q1: Why do we need the config variable to create the clientset, why not directly from the kubeconfig path ?  
	❓ Q2: What is the context package - congext.Background() and the v1.ListOptions magic while creating the clientset ?  
	❓ Q3: The clienset has access to the CoreV1 group (GVK) only and the other groups, the custom group which we would be creating using CRDs ?  

## Day 43:
03-Jan-2023
- Usually, to complete a day's training, I would want to see the output from a program. However, completing this Go Tutorial (https://www.youtube.com/watch?v=YS4e4q9oBaU) over a couple of days, gives me a sense of accomplishment and a great appreciation for the GoLang. A few concepts were a cakewalk and the rest needs more practice - Interfaces, Routines and Channels. The learning of slices, defer/panic/recover keywords, pointers were an easy refresher.Thanks to Michael Van Sickle @vansimke for the wonderful tutorial 👍

## Day 42:
23-Dec-2022
- Hurray, completed my first controller which warns when the image size in a node changes (https://github.com/legorie/nodesize)
- Had a few key learnings:
- (1) Good comfort with GoLang will help understand the existing code. The controller code (examples) need an intermediates understanding of the language - maps, structs, interfaces etc. Still miles to go!
- (2) To understand the datatypes passed, the client-go documentation and the kubectl commands (-o yaml) helped a lot. Next step is understand better the different libraries used in the operator programs

![image](https://user-images.githubusercontent.com/1323423/209407105-7580acf7-6797-4743-828b-a22e2881abbf.png)

## Day 41:
20-Dec-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/queen-attack
- Hands on with Controllers - ekspose by Vivek Singh
- Watched the client go videos from the Kubernetes Pune chapter and KubeCon2017. Wanted to modify the ekspose controller to do check the node image size controller showed by Alena (https://www.youtube.com/watch?v=QIMz4V9WxVc). I understood my shortcomings on the Go langugage, my lack of good understanding of structs and interfaces sent me on a wild goose chase. Now, it is time to get some basics right!

## Day 40:
13-Dec-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/pythagorean-triplet
- Hands on with KubeBuilder - working on the Useless Machine contoller

## Day 39:
03-Dec-2022
- Got a good understanding of CRDs following the self paced training here : https://container.training/kube-selfpaced.yml.html. A great thanks to Jérôme Petazzoni on his work in educating the K8S / Cloud Native community. I remember watching his presentation on Kubernetes Internals (https://www.youtube.com/watch?v=3KtEAa7_duA&t=731s) which gave me the confidence and the understanding to take the CKA exam, which 8 months of training and kubectl mastery could not give me. During my university days (days before youtube and widespread internet), I was on a goose chase to find out how the computer booted from the power button to the login screen. After months and months of digging books and people's knowledge, I got a grasp of the Windows boot process. I had the same level of satisfaction after watching (trying to understand) Jérôme K8S internal presentation.
- 04/Dec/2022 Launched into to the Operators, as I'm to create anything on the cluster, I'm not counting this as an accomplishment for the day :)

## Day 38:
30-Nov-2022
- Discovered a wonderful SaaS site for Linux debugging https://sadservers.com ; great effort by the Fernando Duran, I'm lovin it. Solved the Easy level challenges and learnt a few tricks

## Day 37:
29-Nov-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/pythagorean-triplet

## Day 36:
26-Nov-2022
- Discovered a superb GitHub repo for SRE preparation, lovin it : https://github.com/mxssl/sre-interview-prep-guide
- Covers a lot of ground from deep Linux skills, K8S, DevOps and more

## Day 35:
23-Nov-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/pythagorean-triplet

## Day 34:
21-Nov-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/pythagorean-triplet

## Day 33:
18-Nov-2022
- Spend a whole day setting up again the DEV environment for KubeArmor. Trying kubeadm and minikube did not work on my Ubuntu VMs running on Windows. The Vagrant setup metioned in the developer guide needs an Ubuntu host environment which I don't have. Atlast the setup worked well in k3s. The number of tools available to spin up a K8S environment to learn is pretty impressive

## Day 32:
17-Nov-2022
- DevOps training : Practised the Talisman tool which can detect sensitive information in the code on pre-commit or pre-push

## Day 31:
16-Nov-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/phone-number

## Day 30:
13-Nov-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/leap

## Day 29:
12-Nov-2022
- Analysis on the kubearmor client Go code, identified a change in the core Kubearmor code, requested for help from the authors

## Day 28:
11-Nov-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/pascals-triangle

## Day 27:
09-Nov-2022
- Started reviewing the code for kubearmor-client to add the Host Visibility level

## Day 26:
08-Nov-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/sum-of-multiples

## Day 25:
06-Nov-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/wordy

## Day 24:
05-Nov-2022
- Started DevSecOps training in KodeKloud

## Day 23:
03-Nov-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/armstrong-numbers

## Day 22:
03-Nov-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/protein-translation

## Day 20:
01-Nov-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/sieve

## Day 19:
31-Oct-2022
- Found an issue to work on and provided my first take on the issue [#199](https://github.com/kubearmor/kubearmor-client/issues/199). I'm hoping to add value by fixing this requirement


## Day 18:
28-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/word-count

## Day 17:
26-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/perfect-numbers

## Day 16:
25-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/triangle

## Day 15:
24-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/gigasecond
- Read about Red Hat's UBI images. My fav project has been looking to get its image to be RH certified. I read the RH UBI eBook to learn more about RH's presence in the containerization space. Even having worked on the OpenShift environment for the past 2 years, this book has a lots of information.

## Day 14:
22-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/isbn-verifier

## Day 13:
21-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/reverse-string

## Day 12:
20-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/roman-numerals
- Had a good experience with my favorite OpenSouce project KubeArmor. I saw an issue which I had the knowledge to help, Issue [#942](https://github.com/kubearmor/KubeArmor/issues/942) - Helm installation not working. I quickly downloaded the repo, installed the Helm chart, replicated the issue. Luckily, was able to figure it out to (it was a good-first-issue), fixed it by comparing it with the correct REPO URLs in other deployment methods and was ready to submit my request to pick the issue. Then, I noticed that another contributor had already submitted the fix via another PR. My first work trying to contribute went in vain but I learn that I could help and contribute & more importantly my solution match with that of the contributor. I felt good with my first try; miles to go before I could really add value to the project. 

## Day 11:
19-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/atbash-cipher
- Completed the Chapter 18 of the Kubernetes in Action book

## Day 10:
18-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/pangram & https://exercism.org/tracks/go/exercises/proverb

## Day 9:
17-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/largest-series-product

## Day 8:
16-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/nucleotide-count

## Day 7:
15-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/anagram
- Reading the Chapter 18 of Kubernetes IN ACTION by Marko Lukša. This chapter has a cleared a long time confusion of mine on Group, Version & Kind

## Day 6:
14-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/etl & https://exercism.org/tracks/go/exercises/luhn

## Day 5:
13-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/isogram/ & https://exercism.org/tracks/go/exercises/difference-of-squares & https://exercism.org/tracks/go/exercises/space-age

## Day 4:
12-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/raindrops/ & https://exercism.org/tracks/go/exercises/scrabble-score

## Day 3:
11-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/grains
- Participated in 3 Clash of Code in CodinGame : Ranked 2/8 (Shortest code challenge), 4/6 (# of diagonals in a polygon) , 7/8 (Shortest code challenge)

## Day 2:
10-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/hamming
- Learning about KubeBuilder | TGI Kubernetes 083

## Day 1:
09-Oct-2022
- Hands on with Go | https://exercism.org/tracks/go/exercises/welcome-to-tech-palace


---
Thanks to : 
- For the idea to blog & format | https://aswinbarath.github.io/100-days-of-code-challenge/
