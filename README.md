# Abel Vela · Whitestone

Responsive senior protection website. The public page lives in `index.html`; the React files are unused starter files. Styles are included in the page, with no external font or Tailwind CDN dependency.

## Development

```sh
npm ci
npm run dev
```

## Production

```sh
npm run build
npm run preview
```

Deploy the generated `dist/` directory using the existing hosting setup.

## Scheduling

All primary “Schedule call” links point to `#schedule`. That section embeds the existing GHL booking calendar:

https://link.uigus.com/widget/bookings/family-protection-call

A direct link is included above the calendar as a fallback. When changing calendars, update both the iframe URL and the fallback link in `index.html`. Appointment length, availability, time zones, form fields, and confirmations are managed in GHL. The website does not publish a contact phone number or include telephone links. Phone information requested by GHL is managed separately in that service.

## Accessibility and mobile behavior

- Readable system fonts, 18px body text, high contrast, and 52px or larger primary actions.
- Persistent mobile scheduling action with space reserved below the page.
- Responsive cards and a comparison table that stacks on small screens.
- Skip link, visible keyboard focus, descriptive iframe title, and native FAQ disclosures.
- Reduced-motion preference respected; no rotating headlines or booking modal.
- Optimized WebP images in `public/`; the original image files remain as source assets.

The embedded calendar is a third-party interface. Its internal design and accessibility must be maintained in GHL.
