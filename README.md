# 051 · Pace + Log

**AppADay #051** — The complete running companion. Pace + Log unifies the Pace Planner (Day 049) and Training Log (Day 050) into one cohesive app, then goes well beyond both.

## Features

### Plan Tab

**Plan Setup**
- Race distance selector: 5K, 10K, Half Marathon, Full Marathon, 50K
- Goal time input with live pace-per-mile preview
- Fitness level selector (Beginner, Novice, Intermediate, Advanced)
- Training style selector (Balanced, Polarized 80/20, Galloway Run-Walk, Conservative)
- Long Run Day picker — anchor the week's long run to any day of the week
- Days Off picker — mark permanent no-run days; workouts shift or mileage redistributes

**Plan Date Modes**
- From Start Date — enter when training begins; plan runs forward from there
- From Race Date — enter race day and the app counts back the full plan length, snapping to the correct Monday start; race week places the race on the actual race weekday

**Smart Plan Generation**
- Mid-week onramp: if the start date is not a Monday, a partial "Onramp" week bridges from the start date to the following Monday with easy alternating runs — no quality work, no long run
- Base training: if the plan start date is further out than today, base training weeks are automatically prepended, ramping from ~55% to ~90% of Week 1 mileage so training begins immediately
- Week-by-week accordion with daily workouts, mileage, descriptions, and date labels
- Weekly mileage ramp chart showing the full progression arc

**Active Plan Features**
- Plan locks after generation — inputs become read-only with a Change Plan button that confirms before resetting
- One-off weekly day-off overrides: tap "+ Day Off" on any week, mark a day unavailable, and the app shifts that workout to the nearest free slot or redistributes the mileage across remaining easy days
- Plan view is fully restored on every page load — switching back to the Plan tab always shows the full week accordion

### Log Tab

**Today's Workout Card**
- Appears at the top of the Log tab when a plan is active
- Shows today's prescribed workout type, title, description, and target mileage
- "Log This Run" or "Log Cross-Training" button pre-fills the form with today's date and workout type
- Accounts for weekly overrides — if today's run was shifted or removed, the card reflects it

**Stats and Tracking**
- Total miles, total runs, this-week miles, and average pace
- This-week dot tracker: run days show blue with mileage, cross-training days show purple "XT", rest days show a dash
- Weekly mileage chart: bar or line view, 1W / 2W / 4W / 12W / 26W / All ranges, bars colored by dominant workout type

**Run Logging**
- Workout types: Easy, Long Run, Tempo, Interval, Race, Cross-Train, Rest
- Cross-training sessions are logged separately from rest — they count toward total runs, show a purple pill in the history table, and get their own encouragement messages
- Date, distance (optional for cross-training), duration, feel rating, and notes
- Fuel tracking: log what you took and when, with saved presets
- Shoe tracking: add pairs, set active shoe, logged automatically on each run
- Full run history table with inline edit and delete
- Run detail modal with full workout info

**Post-Run Encouragement**
- After logging any active session (including cross-training), a contextual modal appears
- Pace comparison uses the prescribed pace for the workout type — easy/long runs compare against easy pace, tempo against tempo pace, intervals against interval pace; cross-training skips pace comparison entirely
- Going too fast on an easy day surfaces a gentle caution rather than praise

### The Bridge: Pace Reference Strip

A persistent amber strip between the tabs shows goal pace, easy pace, and race distance once a plan is active. Survives page reloads. Every run detail modal shows a comparison badge — how many seconds faster or slower the logged pace was versus the prescribed pace for that workout type.

## Stack
Single-file vanilla HTML/CSS/JS. No frameworks, no build tools. GitHub Pages deployable.

## Part of AppADay
Built by Augustine Iacopelli · [Portfolio](https://augustineiacopelli.github.io/appaday/)
