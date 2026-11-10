# Market Events

A calendar feed with the dates that move markets: central bank decisions, inflation and jobs data, political and geopolitical events, crypto listings and token unlocks. Subscribe once and the events show up in your calendar next to your own appointments, each with a short note on what's expected and links to the sources.

The feed is updated every morning. New events get added, moved dates get fixed, and after an event has happened its note gets one line with the outcome.

## Subscribe

```
webcal://danieljancar.github.io/market-calendar/events.ics
```

**iPhone and iPad:** Settings > Apps > Calendar > Calendar Accounts > Add Account > Other > Add Subscribed Calendar, then paste the address. On older iOS versions it's under Settings > Calendar > Accounts.

**Mac:** open Calendar, File > New Calendar Subscription, paste the address. Set Location to iCloud if you want it on your phone too, and Auto-refresh to every hour.

**Google Calendar:** Other calendars > + > From URL, and use `https://danieljancar.github.io/market-calendar/events.ics`. Google refreshes subscribed calendars only every few hours, sometimes less.

**Outlook:** Add calendar > Subscribe from web, same https address.

Times are stored in UTC, so your calendar shows them in your own time zone.

## What an event looks like

An event with a known time, like a rate decision, is a timed event:

```
FOMC rate decision
Wed 9 Dec 2026, 20:00 to 21:00 (Zurich time)

Markets price a 25 bp hike after the hot October CPI.

The Fed held rates at the last meeting and Powell said further moves depend on
inflation. A hike in line with pricing is mostly priced in; a hold would likely lift
stocks and crypto, a 50 bp move would hit both. Gold tends to drop on a hawkish
surprise.

Federal Reserve meeting calendar: https://www.federalreserve.gov/monetarypolicy/fomccalendars.htm
```

Events without a fixed time, like negotiations or a summit, are all-day events and can run over several days:

```
US and Iran nuclear talks, second round
Fri 20 Nov to Sun 22 Nov 2026, all day

Delegations meet in Oman. A deal would ease sanctions on Iranian oil, which tends to
push crude lower; a breakdown usually does the opposite.
```

The examples show the format. The dates and notes in the feed are the real ones.

## What's in it

Each event has a category, which most calendar apps show or let you search for:

| Category | Examples |
| --- | --- |
| central bank | FOMC, ECB, SNB, Bank of Japan decisions and minutes |
| macro | CPI, PPI, payrolls, jobless claims, GDP, PMI |
| politics | elections, budget and debt ceiling deadlines, tariff dates, court rulings |
| geopolitics | negotiations, summits, sanctions deadlines |
| crypto | exchange listings, token unlocks, ETF decisions, network upgrades |
| stocks | earnings of large companies, index rebalances |

The calendar keeps events from the last 60 days, so you can look back at what happened.

## Where the data comes from

Dates come from the official sources first: central bank calendars, statistics offices like the US Bureau of Labor Statistics, exchange announcements and government press releases. Expectations and forecasts come from public market coverage and are named with who made them. Every event links to where its date and numbers come from, the official source first.

The feed is put together once a day and checked against the previous days, so a moved date gets fixed in place instead of showing up twice. Nothing in it is tracked or personalised, and the feed doesn't know who subscribes.

## Files

`events.ics` is the feed, a standard iCalendar file (RFC 5545). Each event keeps a stable ID, so updates change the existing entry in your calendar instead of adding a copy.

## Disclaimer

The notes describe what markets expect and how they reacted before. They aren't investment advice. Dates can change at short notice, so check the linked source before you act on one.
