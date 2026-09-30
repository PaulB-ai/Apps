# Lean Plan

A personal 12-week fitness programme built as a phone web app. The goal is to tone up, lose belly fat, get fitter and then stay that way. It mixes gym and home training over 3–4 days a week, tracks weight and waist, and plays your workout playlist.

## The programme

| Session | Where | What | Time |
|---|---|---|---|
| **A** Full body strength A | Gym | Goblet squat, lat pulldown, dumbbell bench press, seated cable row, Romanian deadlift, plank, then an incline treadmill walk | ~45 min |
| **B** Bodyweight circuit | Home | Squats, incline push-ups, glute bridges, reverse lunges, supermans, mountain climbers, plank, bicycle crunch, all timed | ~30 min |
| **C** Full body strength B + intervals | Gym | Leg press, incline dumbbell press, one-arm row, reverse lunge, shoulder press, cable woodchop, dead bug, then rowing intervals | ~50 min |
| **D** Cardio & core (optional 4th day) | Home | Low-impact cardio circuit, then a brisk walk outside | ~35 min |

Suggested week: **Mon A · Wed B · Fri C** (plus **Sat D** on 4-day weeks). Any days work if the two gym sessions have a day between them.

| Weeks | Phase | Gym | Home circuit |
|---|---|---|---|
| 1–4 | Foundation | 2 × 12–15 | 2 rounds, 30 s on / 30 s off |
| 5–8 | Build | 3 × 10–12, intervals start | 3 rounds, 40 s on / 20 s off |
| 9–12 | Burn | 3 × 8–12, heavier | 4 rounds, 45 s on / 15 s off |
| 13+ | Maintain | 3 × 8–12 | 3 rounds, 45 s on / 15 s off |

Progression rule: when you reach the top of the rep range on every set with good form, go up to the next weight.

Belly fat comes off as your overall body fat drops. You can't target it with sit-ups. The training builds muscle and fitness; a small calorie deficit, enough protein, 8–10k daily steps and good sleep do the rest. The Plan tab covers this in more detail.

Check with your GP before starting if you have a heart condition, high blood pressure, joint problems or other health concerns.

## Nutrition

The **Food** tab pairs the training with a meal plan built for the same goal: lose fat, keep and build muscle.

- **Daily target**: calories from the Mifflin-St Jeor formula × your day-to-day activity, minus up to 500 kcal (never more than 20%) for steady fat loss of about 0.4–0.5 kg a week. Protein is 1.6 g per kg of body weight (capped at a BMI-27 reference weight). The target updates each time you log your weight and switches to maintenance calories in the Maintain phase.
- **7-day meal plan**: breakfast, lunch, dinner and two snacks, all under 20 minutes. No tuna, cauliflower or swede. Portions scale so each day lands on your target, and every meal can be swapped for another of the same type.
- **Shopping list** for the week at your portion sizes, grouped by aisle, with tick-boxes.
- **Daily habits**: water, fruit and veg, protein, no sugary drinks.
- **Guide**: eating around workouts, alcohol, sleep, stress, eating out, and what to change if your waist stops going down. The app flags a 3-week stall automatically.

These are estimates for healthy adults. Speak to a GP or registered dietitian first if you have a medical condition, take regular medication, or have a history of disordered eating.

## Features

- **Today**: current week and phase, sessions done this week, your next session, latest check-in.
- **Workout player**: warm-up, each exercise with form cues, tap-to-complete sets with an automatic rest timer, a timed circuit for home sessions, interval and steady-cardio timers, cool-down. Beeps for the last 3 seconds and each change, and keeps the screen awake.
- **Music**: save Spotify or YouTube playlist links. During a workout tap **Open** to play in the Spotify/YouTube app in the background, or **Show player** to play it inside the app.
- **Progress**: log weight and waist, see trend charts, change since you started, and waist-to-height ratio (under 0.50 is a healthy target).
- **Food**: calorie and protein target, 7-day meal plan with swaps, shopping list, daily habits.
- **Settings**: start date, 3 or 4 days a week, sex/age/activity for your calorie target, kg/lb and cm/inches, playlists, backup and restore.

Data stays on your phone in the browser's local storage. Use **Settings › Copy backup** now and then.

## Using it on your phone

The app is plain HTML, CSS and JavaScript with no build step. To install it:

1. Host the folder over HTTPS. The easiest option is GitHub Pages: repository **Settings › Pages**, source **Deploy from a branch**, pick the branch and `/ (root)`.
2. Open the Pages link on your phone.
3. **iPhone (Safari)**: Share › *Add to Home Screen*. **Android (Chrome)**: menu › *Install app*.

It then opens full-screen from your home screen and works offline.

To try it on a computer: `python3 -m http.server` in this folder, then open http://localhost:8000.

## Files

- `index.html`: the whole app (programme data, views, workout player, timers, charts)
- `manifest.webmanifest`, `sw.js`: installable app and offline support
- `icons/`: app icons
