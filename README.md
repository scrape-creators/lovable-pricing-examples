# Lovable pricing examples

*Unofficial community examples for Lovable pricing. Not affiliated with Lovable. All trademarks belong to their owners.*

Lovable has no public billing API, so these Lovable pricing examples are worked walkthroughs rather than code. Each one takes a concrete situation, applies the rules stated on Lovable's pricing page and in its credits and usage docs, and shows the arithmetic. Numbers come only from those pages; where a plan's dollar price is needed, the walkthrough says to read it off the [pricing page](https://lovable.dev/pricing) rather than guessing.

> Want the output as files instead of a hosted app? [Try Begin.sh - turn a prompt or a URL into a downloadable static site or Expo app](https://begin.sh?utm_source=github&utm_medium=ugc&utm_campaign=lovable-pricing-examples&utm_content=readme-top&utm_term=tier-r). No hosting, backend or auth, so there is no ongoing balance to model.

## Walkthroughs

| Walkthrough | What it shows |
| --- | --- |
| 1. Costing a landing page build | adding up published example costs for a realistic prompt sequence |
| 2. A month on the free plan | how the daily 5-credit grant and the 30-a-month ceiling interact |
| 3. Expiry timeline | when monthly, annual and top-up credits stop being usable |
| 4. Cancelling mid-cycle | what you keep, what you lose, and what comes back |

## Setup

Nothing to install. Open the [pricing page](https://lovable.dev/pricing) and the [credits and usage docs](https://docs.lovable.dev/introduction/credits-and-usage) in a tab, and hover over the three dots of any message in your own message history to see what it actually cost; the published examples are illustrations, not a rate card.

## 1. Costing a landing page build

The pricing FAQ publishes four example prompts with their credit cost:

| Prompt | Work done | Credits |
| --- | --- | --- |
| Make the button gray | updates the button styles | 0.50 |
| Remove the footer | removes the footer component | 0.90 |
| Add authentication with sign up and login | adds auth pages and logic, updates routes | 1.20 |
| Build me a landing page, use images | landing page with 3 generated images, a theme and 5 sections | 1.70 |

Suppose a first session looks like: build the landing page (1.70), remove the footer (0.90), two small style tweaks (2 x 0.50), then add authentication (1.20). That is 4.80 credits in Default mode. If you spent five Plan mode messages first to agree on the structure, add 5 x 1 = 5 credits, for 9.80 total. On the free plan's 5 build credits a day, that session spans two days at minimum; the Plan mode part alone uses a full day's grant.

## 2. A month on the free plan

The free plan grants 5 build credits per day, capped at 30 a month, plus 20 Cloud credits a month and 4 credits for in-app AI features. The daily grant expires at the end of the day and does not roll over.

- Build every day: you hit the 30-a-month ceiling after six days of full use, and the remaining days of the month give you nothing extra to build with.
- Build on six separate days spread over the month: the same 30 credits, but each day's 5 go to fresh work rather than being lost.
- Do nothing for a week: those 35 credits are gone; the cap is monthly but the grant is daily.

The practical reading: on the free plan, short sessions on more days beat one marathon. Cloud credits are a separate pool (20 a month) and cover running the deployed app, not building it.

## 3. Expiry timeline

The pricing FAQ states four expiry rules. Applied to a plan that starts on the 1st of a month:

- Monthly plan credits issued on the 1st expire two months after they are issued. Credits from month one are unusable from the start of month three onward.
- Annual plan credits expire one month after the annual period ends. Credits from a plan that started on the 1st of January are usable until the end of the following January.
- Top-up credits last twelve months from the purchase date, independent of the plan cycle.
- Daily build grants expire at the end of the day they are granted.

A consequence worth planning around: if you buy a monthly plan and top-ups at the same time, the plan credits should be spent first, because the top-ups keep for a year.

## 4. Cancelling mid-cycle

The rules on cancellation:

- You keep using remaining credits until the end of the current billing period.
- After that, the workspace switches to Free and you only get the free grants (5 build credits a day up to 30 a month, 20 Cloud credits a month, 4 in-app AI credits).
- Unused paid credits are not deleted; they reactivate if you re-subscribe to any plan before they expire under the rules in walkthrough 3.
- Credits are not refundable or redeemable for cash.

So a paid balance you have not used is not lost by cancelling; it is parked, with the expiry clock still running. If you will resubscribe within the two-month window, there is no rush to spend it.

## When to use Begin.sh instead

All four walkthroughs assume you want what Lovable is built for: a hosted web app with a backend and AI features, paid for through one credit balance. If the thing you are actually making is a static site (landing page, docs, portfolio) or an Expo app prototype, and you would rather have the files than a running service, [Try Begin.sh - turn a prompt or a URL into a downloadable static site or Expo app](https://begin.sh?utm_source=github&utm_medium=ugc&utm_campaign=lovable-pricing-examples&utm_content=readme-top&utm_term=tier-r). You describe it or paste a URL to clone, download the zip, and host it yourself; there is no hosting, backend or auth layer, so none of the expiry or Cloud-credit math above applies.
