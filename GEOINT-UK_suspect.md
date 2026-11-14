# UK Suspect: Geoint and osint challenge

**Type:** GEOINT and OSINT

> Challenge from the [OSINT Industries CTF](https://ctf.osint.industries/challenges).

## What we know

- The photo was taken somewhere in England
- The goal is to find the exact coordinates of where it was taken

## Step 1: Checking the metadata

I first checked the metadata using the [image metadata manager](https://github.com/viktorya-mk/osint-toolkit) I built. It didn't turn up anything useful, so I moved on to the picture itself.

## Step 2: Analysing the picture

A lot of details caught my eye, and I used them to work out the coordinates: a leaning tree, a building with balconies and dark awnings, a restaurant terrace with umbrellas and plants, and a curved parking bay along the street.\
<img height="800" alt="image" src="https://github.com/user-attachments/assets/f415ac0c-649e-454a-9d01-0b09a4eee41a" />


## Step 3: Reverse image search

I ran a reverse image search with a cropped image of the building, and added that it was in England to the search. It returned The Waldorf Hilton hotel in London, and on closer inspection everything matched.\
<img height="742" alt="image" src="https://github.com/user-attachments/assets/9a78c88f-e609-4f7c-ae29-e9d24aac072d" />


The picture was taken from across the street.

## Step 4: Finding the exact spot

On Google Maps, much of the area was hidden by buses and traffic, so I used another map to see more of the surroundings and work out where the photographer stood. I used [Mapillary](https://www.mapillary.com/app/?lat=51.512123100000025&lng=-0.1188148999999612&z=19.102212437106672&focus=photo&pKey=601532521312481) to confirm the details, and everything matched the original image: the leaning tree, the curved parking bay, the restaurant plants, the umbrellas and the waiter counter.\
<img width="1152" height="1192" alt="image" src="https://github.com/user-attachments/assets/7377a3eb-26af-4120-9dc2-7279948abf62" />


This is where the picture was taken. The red arrow shows the direction it faces.\
<img width="533" height="607" alt="image" src="https://github.com/user-attachments/assets/8d9b7a8b-08b6-4998-9102-51b00e8cf1af" />


## Result

The photo was taken at **51.51171° N, 0.11889° W** (51.51171, -0.11889), across the street from The Waldorf Hilton in London.
 
<sub>Street-level imagery from Mapillary and Google. Aerial imagery © Google.</sub>
