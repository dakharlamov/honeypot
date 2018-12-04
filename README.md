# Honeypot Experiment

## Honeypot in Use: Dionaea

## Issues Deploying Honeypot

While setting up this Honeypot, I ran into a lot of issues around the hosting of the virtual machine on gCloud (GCP).
The first of such issues was due to an issue in the install script provided with the Modern Honey Network (MHN) fork
that was used in this experiment. Once resolving a git dependency that was bugged, the install was finally able to succeed.
Launching the VM wasn't too difficult but getting it to serve anything on http was difficult. I managed to resolve connection
issues by allowing http traffic to the GCP VM, viewing the status of the servers on MHN, and then forcing my browser to accept
a HTTP connection. Once I was finally able to access the MHN GUI, the rest of the experiment was straight forward from there.

## Some Statistics

- Time to Complete experiment
  - 5 hours
- Number of attacks
  - 1025
- Country with the Most Attacks Outside of the USA
  - China
- Most Attacked port
  - Port 23

## Some Questions

The lingering questions that I still have after completing this experiment are:

- How many systems are actually vunerable to the attacks that I captured during my experiment?
- Do the attackers know that they have fallen for my honeypot?
- How common is it so set up honeypots like Dionaea to fool attackers? If there are many known honeypots in use,
  wouldn't it be possible for an attack to quickly anticipate that they are falling into a honeypot trap?
