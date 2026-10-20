
# Student Leave Requests – Automate Campus Quest (Challenge 2)

## Problem
Faculty manually read, check and approve leave requests.

## Flow summary
1. Manual trigger: student name, email, days, reason
2. Validate inputs → missing details mail → terminate
3. Autonomous agent classifies reason (Medical / Family / Event / Other)
4. Switch routes by category
5. Rules: medical ≤ 5 days, family ≤ 3 days → auto-approve
6. Everything else → faculty review mail
7. Agent error → Terminate (Failed)

## Why each node
- Agent: understands free-text reasons
- Decision: simple numeric limit
- Switch: more than two categories
- Terminate (Failed): error handling

## Sample data
Which parts use sample data (list them here)

## Test cases
See docs/test-cases.md
