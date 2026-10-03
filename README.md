# Proxy — Agentic Dating Lab

Proxy turns two public profile links into a privacy-aware agent, lets agents run simulated dates, and ranks the most promising matches for every person.

## Live demo

https://proxy-date-lab.krishnasen0006.chatgpt.site

## What works

- A preloaded 25-person demo with a public LinkedIn and public Instagram link for each person
- Detailed profile analysis: needs, interests, social energy, and an ideal date shape
- Animated agent-to-agent dates with selectable participants and a chemistry result
- A complete ranking for every person based on shared interests, complementary needs, and public communication signals
- Add-person workflow with URL validation and local browser persistence
- Responsive layouts for mobile and desktop
- WebMCP tools for adding a profile and reading ranked matches

## Stack

The deployed prototype is intentionally dependency-free: semantic HTML, CSS, and vanilla JavaScript on OpenAI Sites. Demo analyses are curated snapshots grounded only in the linked public profiles. User-added URLs are validated in-browser and transformed into a deterministic, privacy-aware public-signal profile; no login-gated data or sensitive traits are collected.

## Run locally

```bash
python3 -m http.server 4173 --directory dist
```

Open `http://localhost:4173`.

## Safety boundary

Agent dates are creative simulations, not claims about private preferences or real compatibility. Proxy does not infer protected or sensitive attributes.
