# Definition of done

You are done when a reviewer can do all of this using only your repo, your live URL and the admin login you send us.

## As a customer

1. Open the live URL, sign up as a new user, and get a new organization.
2. Log out and log back in. Request a password reset and finish it.
3. Invite a teammate and have them join with a role. If you do not send real email, show the invite link on screen or in the logs and tell us where.
4. As the teammate, create a ticket, add comments and change its status.
5. Ask for an AI draft on the ticket and see it. If the AI service is slow or fails, see a clear message, not a crash.
6. See how many drafts the organization has used against its plan limit.
7. Reach the free plan limit and be stopped with a clear message.
8. Upgrade to the pro plan through Stripe checkout (test mode) and see the plan and limits change.
9. Downgrade or cancel and see the limits come back.
10. Try to open another organization's ticket by guessing its id and be refused. A second signup stays completely separate from the first.
11. As an agent, try owner or admin actions (invite, billing) and be refused.

## As the platform admin

12. Log in to the admin panel with the admin login. It is separate from customer logins.
13. See every organization with its plan, seats, usage and subscription status.
14. Open one organization and see its users and recent activity.
15. Change a plan's limits (for example drafts per month) and see the change take effect.
16. Suspend and re-enable an organization. Suspended users cannot use the app.
17. Configure the AI settings (provider, model, or on and off) from the panel.
18. See recent errors and alerts.

## As an engineer reading your work

19. One documented command runs the app locally, and the tests run and pass.
20. CI runs on a push and shows green, and deploys happen only after green.
21. A server error is logged without secrets and sends one alert, not a flood.
22. Your notes explain each decision and why, and show how you checked every item above and what you could not check.
23. Your tech stack choices are explained, including why and what you ruled out.
24. A diagram shows how everything interacts, as an architecture or a code flow.
25. Anything you did not finish is listed with what you cut and why, based on your time.

Please seed a little demo data (an organization with a few tickets and a free and a pro example) so we can see the app working right away.
