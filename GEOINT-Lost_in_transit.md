# Lost in Transit: Finding a Train Station and the Time of Day

**Type:** GEOINT and OSINT

> Challenge from the [OSINT Industries CTF](https://ctf.osint.industries/challenges).

## The questions

1. Which train station was this photo taken in?
2. At what time was it taken, within a window of two hours?

## Step 1: Checking the metadata

Before anything else, I checked the photo's metadata for a location or any other useful detail, using the [image metadata manager](https://github.com/viktorya-mk/osint-toolkit) I built. It didn't turn up anything useful, so I moved on to the picture itself.

## Step 2: Analysing the picture

A few things stood out: a French flag on top of the station roof, a bag with French text, and what looks like a warm season.

<img height="700" alt="image" src="https://github.com/user-attachments/assets/fca4891b-c3b1-4de8-89ac-11cc8022d9ca" />


## Step 3: Which station

I started with a reverse image search. It led me to an [article from La Provence](https://www.laprovence.com/article/societe/1671485734306715/il-faut-un-bac-8-en-ferroviaire-depuis-marseille-un-rapport-pointe-la-complexite-du-voyage-en-train-en-europe) with a very similar picture, and its description places it at Gare Saint-Charles in Marseille.

I then confirmed the station with a Google search.

## Step 4: What time of day

With the station known, I needed the time of day. This is the aerial view of the station: the blue arrow shows the direction the photo was taken, and the red arrow shows the direction of the shadows.

<img width="1487" height="917" alt="image" src="https://github.com/user-attachments/assets/e84a07c8-78b7-4535-95b6-2471e2ee2dee" />


I used the sun map [SunCalc](https://www.suncalc.org/) to see where the sun would be in the sky. I assumed a date around mid-July, since the weather looks hot. After experimenting with the time slider, the sun's direction matched the shadows best between about 10:00 and 12:00.

<img width="977" height="1267" alt="image" src="https://github.com/user-attachments/assets/7fbc9c46-4daf-4187-81ac-1cb989ac36aa" />


## Result

The photo was taken at **Gare Saint-Charles, Marseille, France**, between **10:00 and 12:00**.

<sub>Aerial imagery © Google. Sun position from SunCalc.</sub>
