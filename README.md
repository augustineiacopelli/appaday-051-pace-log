# 051 · Pace + Log

**AppADay #051** — The training arc payoff. Pace + Log unifies the Pace Planner (Day 049) and Training Log (Day 050) into a single, cohesive app.

## Features

### Plan Tab
- Race distance selector: 5K, 10K, Half Marathon, Full Marathon, 50K
- Goal time input with live pace preview
- Fitness level and training style selectors (Balanced, Polarized 80/20, Galloway Run-Walk, Conservative)
- Optional plan start date with Monday validation
- Generated week-by-week accordion with daily workouts, mileage, and date labels
- Weekly mileage ramp chart (canvas)

### Log Tab
- Total miles, total runs, this-week miles, average pace stats
- This-week dot tracker with daily mileage
- Weekly mileage chart: bar or line, 1W/2W/4W/12W/26W/All ranges, colored by dominant workout type
- Run entry form: date, distance, duration, workout type, feel, fuel tracking, notes
- Shoes settings: add/track active shoe pair
- Fuel presets: save commonly used gels and snacks
- Full run history table with edit and delete
- Run detail modal

### The Bridge: Pace Reference Strip
After generating a plan, a persistent amber strip appears between the tabs showing your goal pace, easy pace, and race distance. It is restored on page load from localStorage, so it follows you even if you return later. Every run detail shows a pace comparison badge — how many seconds faster or slower your logged pace was compared to your race goal.

## Stack
Single-file vanilla HTML/CSS/JS. No frameworks. No build tools. GitHub Pages deployable.

## Updates Needed
- Error fix to allow fill in runs between training start and today's date breaking run currently.
- Would like to add additional gfx and other engaging elements to improve overall UI.

## Part of AppADay
Built by Augustine Iacopelli · [Portfolio](https://augustineiacopelli.github.io/appaday/)
