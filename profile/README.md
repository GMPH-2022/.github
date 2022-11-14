## Inspiration
One in 10 patients in India dies on the way to hospital and the average arrival time of the ambulance is 45 to 50 minutes.

We conducted a survey among ambulance drivers to gather information about the real challenges faced by them. The worst challenge faced by them is traffic, that can be easily reduced if people are aware that an ambulance is on the way. 

By integrating this feature, all users will get notified and some users may try to help clear the traffic which would help ambulances to get to the destination faster and save many lives.

## What it does

The solution to this problem is to notify people using Google Maps app when an ambulance is nearby or on their way.

The app notifies the users near the ambulance about the position and ETA so that they have enough time to think and act accordingly.

If we are able to notify people about the incoming ambulance then some users might try to clear the traffic and that would help the ambulance to reach destination faster and save many lives.  


## Algorithm
With the prerequisite of India’s latitude and longitude extents, we represent the world map into grids of 1km x 1km as shown. This helps to compute the index of the cell in which the ambulance driver is present.

![gridmap](https://user-images.githubusercontent.com/74011816/201745412-fb6b321a-a996-4bf2-bfe2-a4c6ec19fd84.png)

## How we built it
A survey was conducted among ambulance drivers to gather information about the real challenges faced by them.

The app is built using Flutter for the frontend, Firebase for the backend and used Google Maps Platform APIs to embed Google Maps into mobile apps and to retrieve data from Google Maps.


## Challenges we ran into
- The challenge that we faced was to identify the nearby ambulances.
- Finding ETA between two points was a challenging task since the distance matrix API takes places as input parameters instead of latitude and longitude.
- We could not use the cloud functions in Blaze plan for deleting expired data documents in firestore and instead used the Spark plan.


## Accomplishments that we're proud of
We are proud about implementing the navigation functionality that itself zooms in/out or tilts the map to enhance the user experience.

We designed a computationally efficient grid indexing algorithm to get the nearby users.

Additionally, this was our first long hackathon experience, so we are proud that we were able to finish it within the given time frame along with a huge academic load from the college.

## What we learned
This was our first time using firestore and we learned how to integrate firestore with flutter.

We also learned about the Google maps platform tools and how to customize them.

## What's next for Make Way

Ideally we would like to make this app work for any place in the world, which for now is limited to India only.

The estimated time of arrival of an ambulance can be notified depending on the varying traffic conditions.

We could perform primitive data analysis to extract information such as number of accidents in a unit time, location of maximum occurence of accidents and apply reasoning to obtain useful statistics.
