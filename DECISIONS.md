# GYST Decisions

Last updated: June 8, 2026

## Product Decisions

### Command Is The Main Experience

Decision: Command/Dashboard is the default landing experience.

Reason: GYST should feel like it is running the user's day, not like a set of separate trackers.

### No New Tabs For MVP

Decision: Do not add more tabs right now.

Reason: The app already has enough surfaces. New concepts should be integrated into Command, Schedule, Budget, Health, Focus, Coach, or Profile.

### Next Best Move Comes First

Decision: Next Best Move is the primary hero card.

Reason: The user should know what to do immediately.

### Discipline Score Is A Status Signal

Decision: Discipline Score should be visible but smaller than the action prompt.

Reason: The score supports behavior, but the product should not become a scoreboard-first app.

### Start My Day Is Guided

Decision: Start My Day should be a 3-step flow:

1. Confirm next commitment and biggest risk.
2. Confirm or swap mission items.
3. Start first action.

Reason: A morning flow should reduce decisions, not just display a checklist.

### Daily Mission Formula

Decision: The daily mission has five required categories:

- money
- body
- food
- focus
- life reset

Reason: These categories create a minimum viable disciplined day.

### Swap And Replan Are Allowed

Decision: Users can swap mission items within the same category and replan incomplete items.

Reason: GYST should apply pressure without making the day brittle. Misses should turn into replans, not abandonment.

## Scope Decisions

### Local/Mock First

Decision: Keep the MVP local/mock until the core daily loop works.

Reason: The product risk is habit value, not backend complexity.

### No Bank Sync Yet

Decision: Manual budget and safe-to-spend come before bank sync.

Reason: Bank sync adds cost, complexity, privacy concerns, and integration work. The product should first prove that users want GYST's money guidance.

### No Investing Automation Yet

Decision: Investing remains education/reminders only in V1.

Reason: Automated investing can create legal, compliance, brokerage, fiduciary, and advisory obligations.

### Stability Before Investing

Decision: GYST should push users to build a 2-3 month daily-spending safety net before investing pressure.

Reason: The product philosophy is stability first, freedom second, investing third.

### No Real Phone Lock Yet

Decision: Focus mode and bypass are concepts until platform enforcement is confirmed.

Reason: Deep iOS/Android restriction requires platform-specific APIs, entitlements, or careful native work.

## Calendar Decisions

### Start With Native Phone Calendar

Decision: Use the phone's native calendar first.

Reason: It can include Apple Calendar, Google Calendar, Outlook, school, work, and subscribed calendars without requiring direct provider OAuth on day one.

### Confirm Before Destructive Calendar Actions

Decision: Deleting from GYST can be simple, but deleting from a real phone calendar should require confirmation.

Reason: Calendar deletion is destructive and could remove real commitments outside GYST.

### Calendar Should Feel Like A Planner

Decision: Schedule should support year/month/week/day visibility and full-day time blocks.

Reason: The user wants the clarity of a real planner and Google/Apple Calendar style visibility, without copying proprietary UI exactly.

## Design Decisions

### Dark Mode First

Decision: GYST uses a polished dark-mode interface.

Reason: The product should feel serious, focused, and habit-oriented.

### Progressive Disclosure

Decision: Show the most important action first, then reveal supporting details.

Reason: The target user may struggle with overwhelm and task initiation.

### Pressure With Recovery

Decision: GYST should be firm but allow replanning.

Reason: The tone is "get your shit together," but the product must help users recover after misses.

## AI Coach Decisions

### Coach Should Customize The App

Decision: The AI coach should eventually change profile settings, goals, sleep targets, pressure mode, and mission logic.

Reason: The user wants the coach to think like Codex/ChatGPT and adjust the app live.

### Coach Is Not The Main Interface

Decision: Chat supports customization, but Command runs the day.

Reason: The user should not have to type their issues all day. They should mostly tap, confirm, start, swap, or replan.
