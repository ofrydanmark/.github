# Ofry

Booking-platform for hjemmeservice i Danmark — vinduespudsning, havearbejde,
rengøring, malerarbejde, højtryksrensning, bilpleje, handyman-opgaver og mere.
Kunder booker pålidelige lokale udbydere; udbydere driver deres forretning fra
ét samlet dashboard.

Live på [ofry.dk](https://ofry.dk).

## Repositories

| Repo | Formål |
| --- | --- |
| [service-now-simple](https://github.com/ofrydanmark/service-now-simple) | Kunde- og udbyder-webapp (Vite, React, Tailwind, shadcn/ui) |
| [ofry-app](https://github.com/ofrydanmark/ofry-app) | Mobilapp til kunder og udbydere (Expo, React Native, NativeWind) |

Begge klienter deler én Supabase-backend (Postgres, Auth, Storage, Edge
Functions), med Stripe Connect til udbetaling til udbydere og Stripe Payments
til bookings.

## Stack

- **Frontend** — React, TypeScript, Tailwind / NativeWind
- **Mobil** — Expo Router, EAS Build, native moduler hvor nødvendigt (`react-native-maps`, `expo-notifications`, `@stripe/stripe-react-native`)
- **Backend** — Supabase (Postgres + Edge Functions på Deno), Stripe (Connect + Payment Intents), Resend (transaktionel mail), Google Maps Platform
- **Tooling** — Bun, Lovable til web-iteration, EAS til mobil-builds

## Kontakt

Baseret i Danmark. Kontakt teamet på [hello@ofry.dk](mailto:hello@ofry.dk) for
partnerskaber, support eller henvendelser om jobs.
