# Roller Coaster Designer

## Purpose
- Draw a roller coaster track and ride it. A car starts at the top of the first hill and rolls along the track under gravity, and the app shows its speed and the g-forces on the riders as it goes.

## Inputs
- A track the user draws or shapes by dragging control points, with a smooth curve through them

## Calculations
- The speed the rollercoaster goes based on gravity, the height the rollercoaster starts at, etc.

## Outputs
- Live readouts of speed (mph) and vertical g-force, and a plot of both along the track
- Failure when the car doesn't have enough energy to reach the next crest (it rolls back) or when the g-force goes above 4 g or below -1 g, with the failure point marked on the track
- An animated car that follows the track, with its speed computed from conservation of energy


## Look and Feel
- Colorful and cartoonish, not too detailed but not boring, like something you would see out of the cool math games website
## Features
- Score of the track design based on thrill (time spent above 3 g) while also keeping the design safe
- Physics describer, a pop up that describes the variables and what's happening and why it's happening (as this app may be used for a hs physics class for example)

## Validation
- With no friction, the speed at any point is v = sqrt(2g(h0-h)), where h0 is the height of the starting crest.
- For a valley with radius of curvature R, check app g-force against n = 1 + v^2 / gR

## Out of Scope
- Complex details unnecessary to what I'm getting at with this app