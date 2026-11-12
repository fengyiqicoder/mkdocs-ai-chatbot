# Track events

Page views are counted automatically. Anything else, such as a button click or a sign-up, is an event.

## From JavaScript

Call `tally.event` with a name, and optionally a few properties:

```js
tally.event("signup");
tally.event("purchase", { plan: "pro", value: 49 });
```

Event names are case-sensitive, up to 64 characters. Properties are strings or numbers, at most 10 per event.

## Without JavaScript

Add `data-tally-event` to any link or button, and Tally sends the event when it is clicked:

```html
<button data-tally-event="download">Download</button>
```

## Goals

In the dashboard, open **Goals** and pick an event to turn it into a goal. Tally then shows the conversion rate of each page and each referrer for that goal.
