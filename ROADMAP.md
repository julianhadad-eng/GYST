# GYST Roadmap

## Product Principle

GYST should become the user's daily operating system.

The roadmap should protect this order:

1. Run the day manually with mock/local intelligence.
2. Prove the Command Center habit loop.
3. Add persistence and real accounts.
4. Add integrations.
5. Add automation carefully.

## Phase 1: Command Center MVP

Goal: make GYST useful every morning in under 60 seconds.

Build:

- Refine Start My Day guided flow.
- Make mission completion persist locally by date.
- Add clearer active action state.
- Add basic timer behavior for the first action.
- Show a simple "replan the day" path when a user misses or delays an action.
- Tighten Command layout after visual QA on phone.

Avoid:

- new tabs
- complex dashboards
- backend dependencies
- real phone lock
- bank sync
- investing automation

## Phase 2: Real Local App

Goal: let a pilot user use GYST daily with their own information.

Build:

- Save mission history locally.
- Save user-created schedule blocks locally.
- Improve onboarding profile intake.
- Add editable profile goals.
- Add real manual budget entries.
- Add manual food/protein logging.
- Add weekly review screen or section inside Command/Profile.

Key question:

Does the user return because GYST tells them what to do next?

## Phase 3: Account + Database

Goal: make user data durable across installs/devices.

Build:

- Supabase auth.
- Profiles table.
- Mission history table.
- Schedule blocks table.
- Budget items table.
- Food entries table.
- Discipline score events table.
- Coach memory/context table.

Keep:

- Command as the main surface.
- Integrations optional.
- Manual entry usable without external accounts.

## Phase 4: Calendar Integration

Goal: make GYST aware of real commitments.

Build:

- Improve native phone calendar import.
- Add confirmation before writing to phone calendar.
- Add confirmation before deleting from phone calendar.
- Add conflict detection.
- Add recurring schedule patterns.
- Later, add direct Google Calendar OAuth if needed.

Decision:

Start with the phone's native calendar because it can include Apple, Google, Outlook, work, school, and subscribed calendars without forcing users to choose one provider on day one.

## Phase 5: AI Coach That Changes the App

Goal: let the coach adjust goals, schedule assumptions, tone, and mission logic.

Build:

- Coach can update local profile settings.
- Coach can adjust sleep goal, wake time, priority habits, workout targets, food goals, and pressure mode.
- Coach can explain why a mission was chosen.
- Coach can suggest replans.

Guardrails:

- User confirms meaningful changes.
- Coach does not create bank/investing actions.
- Coach does not pretend to enforce phone locks before platform work exists.

## Phase 6: Money Integrations

Goal: improve accuracy without making the app legally risky too early.

Build:

- Bank sync through a provider like Plaid only after manual budget value is proven.
- Subscription detection.
- Spending categorization.
- Safe-to-spend automation.

Avoid until legal/compliance review:

- automated transfers
- brokerage account opening
- personalized investment advice
- automatic investment purchases

## Phase 7: Device Restrictions

Goal: make focus and distraction control stronger.

Build:

- Notification reminders.
- Widgets.
- Shortcuts/App Intents where possible.
- Screen Time / Android restriction research.
- Emergency bypass with recovery commitment.

Important:

Deep phone restriction is platform-constrained and should not be promised as real until the technical path is confirmed.

## Pilot Success Metrics

Track:

- user starts Start My Day
- user completes first action
- user completes at least 3 mission items
- user checks safe-to-spend before spending
- user logs or plans food
- user completes movement/workout target
- user replans instead of abandoning the day
- user returns the next morning

The MVP wins if users say:

```text
I opened GYST and it told me exactly what to do next.
```
