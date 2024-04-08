# theme-park-simulation

## WHAT IS IT?

The model creates a simulation of an amusement park, focusing on the dynamics of visitor movement and queue management within such an environment. It will model various attractions with differing levels of popularity and simulate the behaviours of varying archetypes of visitors. The simulation will incorporate different queueing strategies, including systems such as virtual or privileged express queues, to analyse and optimise the flow of visitors. By integrating these elements, the simulation seeks to provide insights into queue management, enhance visitor experience, and improve operational efficiency within amusement parks.


## HOW IT WORKS

The visitor makes decision to join attractions based on their archetype and the queue-mode. 


## HOW TO USE IT

setup (button) - creates the theme park (entrance, attractions, activity and pathways.

queue-mode(chooser) - choose the basic, express and priority queue.

passive-prob, leisure-prob, average-prob, enthu-prob and fanatic-prob(sliders) - the five archetypes mix. 

closing-time(slider) - represents the opening hours of the theme park 250 tick = 9 hours

stop-at-closing-time(switch) - stops the model at closing-time referenced from the closing time slider

express-prob(slider) - when "express" is choosen in the queue-mode, represents the chance of a visitor owning an express pass.

priority-pass-limit(slider) - when "priority" is choosen in the queue-mode. The maximum number of priority passes an attractions issues.

satisfaction-threshold(slider) - the point where the visitors will leave the theme park if their satisfaction falls below the satisfaction-threshold.

satisfaction-modifier(slider) - the uility the visitors gets when they successfully finish the attraction. Decreases when the visitors fail to get their ride.

current visitor count(monitor) - a live update of the total current visitors in the park.

unsatsified visitors(monitor) - a live update of the total unsatisfied visitors that visited the park.

number of park visitors(plot) - a live update on number visitors by archetype

average satisfaction levels by archetype(plot) - a live update on the average satisfaction by archetype.

Average Satisfaction Of Normal and Express Pass Holders(plot) - when "express" is choosen in the queue-mode, compares the average satisfaction between the Normal and Express Pass Holders.


## THINGS TO NOTICE

Attractions: 
Ride (eg. rollercoaster) represented by green squares and 4 rides are pre-defined as popular for all visitors.

Activity (eg. meet & greet) represented by yellow triangle and all activities are equally popular for all visitors.

Each of the attactions contains the queue length (Q: basic queue, E: express queue, V: virtual queue).

Park Entrance:
All visitors start from here upon arrival and end here to leave.

Pathways:
Represented by links, visitors can only travel along them to explore.

Attraction Labels:
"Q" show the number of visitors in the standard queue, "E" show the number of visitors in the express queue and "V" show the number of visitors in the virtual queue (priority pass)
 
## THINGS TO TRY

queue-mode(chooser) - choose the basic, express and priority queue. 

passive-prob, leisure-prob, average-prob, enthu-prob and fanatic-prob - the five archetypes mix.

closing-time(slider) - represents the opening hours of the theme park 250 tick = 9 hours

express-prob(slider) - when "express" is choosen in the queue-mode, represents the chance of a visitor owning an express pass.

priority-pass-limit(slider) - when "priority" is choosen in the queue-mode. The maximum number of priority passes an attractions issues.

satisfaction-threshold(slider) - the point where the visitors will leave the theme park if their satisfaction falls below the satisfaction-threshold.

stop-at-closing-time(switch) - stops the model at closing-time referenced from the closing time slider

## EXTENDING THE MODEL

(suggested things to add or change in the Code tab to make the model more complicated, detailed, accurate, etc.)

Simulated Agent Simplification: Increase variety of simulated agent types, including age variation and purchasing power.

Static Environment Assumption: Implement adjustable possibility of attraction downtime and navigation delays into simulation.

Lacking Physical Interactions: Add visitor types that arrive and decide in groups, emulating family gatherings or friend outings.

Predictability of Visitor Arrivals Introduce Poisson distribution data for different days of the week, annual seasons, and notable calendar event days.

Simple Attraction Popularity Effect: Add attraction tags and visitor preference tags (eg. wet, thrill, scenic, sky-high, branded, etc.) that can be matched and affected by the weather or time of day. Additionally, allow all attractions to have adjustable general popularity effects to emulate social media to a certain extent.