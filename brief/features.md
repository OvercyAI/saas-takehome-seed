# Feature list

Everything below needs to work end to end. The [definition of done](definition-of-done.md) shows how a reviewer will check it.

1. **Authentication.** Sign up, log in, log out, password reset. Sessions are secure. Repeated bad logins are slowed or blocked.
2. **Multitenancy.** Each company is its own organization. People belong to an organization with a role (owner, admin or agent). Owners and admins can invite people. One organization can never see or change another organization's data.
3. **Tickets.** Create, list, view and update tickets, and add comments. Everything is scoped to the organization.
4. **AI drafts.** An agent can ask for an AI-written reply to a ticket. Use the AI product of your choice and tell us why you chose it. Handle slow responses and failures gracefully. One organization's data must never end up in a prompt for another. Record usage and cost.
5. **Billing with Stripe.** A free plan (50 AI drafts per month, 3 seats) and a pro plan (1,000 drafts per month, 25 seats). Checkout, webhooks, subscription state, usage counted against the plan limit, upgrade and downgrade. Stripe test mode is fine. Use your own free test account, or a stand-in if you prefer, and explain it.
6. **Platform admin panel.** A separate admin login for the Deskly team, with a panel to view and configure the platform: organizations, users, plans, usage, billing state, AI settings and recent errors.
7. **Security.** Validate input, keep secrets out of the code and the logs, set sensible headers and CORS, return safe error messages, and use least privilege.
8. **CI/CD.** A pipeline that runs your checks on every change, and a deploy path that only runs when the checks are green.
9. **Verification and QA.** Automated tests, plus a documented and repeatable way to check the running app end to end. Show us what you checked and what you did not.
10. **Skills and agent rules.** Rules, skills or instructions that make an AI coding agent productive and safe in your codebase.
11. **Error logging and notifications.** Structured logs that do not leak sensitive data, and an alert when the server errors, without flooding anyone.
