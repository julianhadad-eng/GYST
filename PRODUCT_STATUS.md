# GYST Product Status

Last updated: June 8, 2026

## Current Build

GYST is an Expo React Native TypeScript MVP focused on helping users run their day through a Command Center. The current app is local/mock-first with Supabase placeholders for future auth/database work.

The app now opens directly into the main tab experience with the first tab labeled Command.

## Current Core Experience

The Command Center is the main experience.

It currently shows:

- Next Best Move as the primary hero action
- Discipline Score as a smaller status card
- Next calendar/schedule block
- Safe-to-spend amount
- Food/protein target
- Fitness target
- Focus block recommendation
- Biggest risk today
- Start My Day guided flow

The intended product feel is:

```text
Here's the plan. Here's the risk. Start this now.
```

Not:

```text
Here are your metrics.
```

## Start My Day Flow

Start My Day is local/mock only.

It has three steps:

1. Confirm next commitment and biggest risk.
2. Confirm or swap today's mission items.
3. Start first action.

The daily mission includes:

- 1 money action
- 1 body action
- 1 food action
- 1 focus action
- 1 life reset action

Mission items can be:

- completed
- swapped for another option in the same category
- replanned if incomplete

Completing mission items updates the visible Discipline Score locally.

## Tabs

Current tabs:

- Command
- Schedule
- Budget
- Health
- Focus
- Coach
- Profile

No new tabs should be added for the current MVP. Command should act as the operating system, while the other tabs hold deeper supporting tools.

## Current Data State

The app uses local mock data and local profile state.

Implemented:

- mock budget data
- mock schedule events
- mock food/macros data
- mock focus plans
- mock discipline metrics
- local profile state with AsyncStorage
- Expo calendar read/write concept
- Supabase client placeholder
- Supabase Edge Function placeholder for future AI coach

Not implemented yet:

- real user accounts
- persistent mission history
- backend database writes
- real bank sync
- real brokerage/investing automation
- real phone locking
- production AI coach behavior

## Technical Health

Latest TypeScript check passed:

```bash
npm run typecheck
```

## Current Risks

- The Command Center has not been visually QA'd on a physical device after the latest guided Start My Day refinement.
- Mission completion is local screen state only and resets when the screen/app reloads.
- Calendar deletion currently removes/hides blocks from GYST, but true phone calendar deletion should require confirmation before being added.
- The app is still a product prototype, not production-ready.

## Next Best Product Question

The next product question is whether the Command Center is understandable in under 60 seconds for a new user:

- Do they know what to do first?
- Do they understand why GYST picked it?
- Can they adjust the plan without escaping the flow?
- Does the pressure feel helpful instead of overwhelming?
