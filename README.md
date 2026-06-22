# SMEDTEC Studio — Demonstration

An interactive illustration of SMEDTEC Studio — a bespoke product, supplier and compliance system that SMEDTEC builds for a client, on the client's own infrastructure.

It has two linked views, and you can switch between them at any time using the toggle in the top bar (**How it works · What you get**):

* **How it works** — *Connected Compliance*: a walkthrough of how Studio wires a client's tools, suppliers and evidence into one live layer that reasons over the evidence but never decides for them.
* **What you get** — the Studio itself: a fully interactive illustration of the product, across its product, supplier and compliance views.

> **Note:** This is a demonstration built on a fictional brand and anonymised sample data. It is for representation only and is not a live compliance system.

## Live demo

https://smedtec.github.io/studio-demo/

The site opens on **How it works**; use the toggle in the top bar to move to the Studio at any time.

## What SMEDTEC Studio is

A single system that brings three disciplines together — product management, supplier management and compliance — built around a client's range rather than bought off the shelf.

* Delivered as a project, not a subscription.
* Built on the client's own infrastructure and connected to the tools they already use.
* Owned outright by the client at the end of the term — the software, the data and the IP. No subscription, no licence, no lock-in.
* The only ongoing cost is the negligible, pass-through cost of running the back-end tools.

## How it works — Connected Compliance

The view the site opens on. It shows the shape of the system: inputs on the left — suppliers and OEMs, test labs, commerce/PIM and market rule changes — flow into the central Studio layer, which reasons over the evidence and pushes work back out to the tools where it lands, such as Slack and ClickUp. Every decision stays with the client; the AI surfaces what's affected and drafts the action, but never approves it.

In this view you can:

* **Run a flow** — pick a scenario and press play to watch it move through the system step by step.
* **Switch your stack on or off** — toggle the connected tools to see how the layer adapts.
* **Set the company name** — under "Connected for", to personalise the walkthrough.
* **Take the tour** — a short guided introduction to each part of the diagram.
* **Copy share link** — captures the current state in the URL so it can be shared exactly as shown.
* **See the AI draft an action** — then choose to approve it or send it for review, illustrating "AI reasons, you decide".

## What you get — the Studio

When this view loads it opens on a choice, because every Studio is built to order — there is no single "default" view:

* **See a sample setup** — jump into a fully populated Studio for a fictional consumer-health brand: posture map, suppliers, claims and project board.
* **Build your own** — a short setup wizard asks for your company name, the product types you make, the systems you use and the priorities you're facing, then assembles a Studio from your answers. It carries your company name, seeds example SKUs for each category, shows your chosen systems connected, and surfaces your priorities. Rebuild at any time to run it again.

This is illustrative: a real build is made from scratch around your actual products and systems.

### What you can do in the Studio

* Explore the Studio across Product, Supplier and Compliance, plus the portfolio posture map and project board.
* Use the Studio Assistant — open it from the floating button (bottom-right). It's a scripted illustration of how an in-Studio assistant would work, including an agentic "set up a starter portfolio" flow that creates products, connects a tool and drafts tasks step by step. Responses are scripted to show intent — it is not a live AI.
* Rename the workspace — click the company name in the top bar.
* Add a product — "+ Add product" on the Product tab.
* Add a task — "+ Add task" on the project board.
* Connect a tool — click any integration tile (ClickUp, Slack, Monday.com, Airtable, Excel, etc.) to connect or disconnect.

Changes are saved in your own browser only, so they survive a refresh and never affect other viewers. Use **Reset demo data** (bottom of the sidebar) to restore the sample, or **Rebuild** to run the wizard again.

## How it's built

* Two self-contained pages — `index.html` (the *How it works* / Connected Compliance walkthrough) and `studio.html` (the Studio) — each built from HTML, CSS and vanilla JavaScript.
* They cross-link with relative paths, so the toggle works wherever the pair is hosted together.
* No build step, no dependencies, no backend. Fonts load from Google Fonts.
* Session state is held in the browser via `localStorage` (versioned, so updates never load incompatible saved data). The Connected Compliance view also supports a shareable link that carries its state in the URL.

## Updating the site

The site lives at the repository root, published with GitHub Pages: `index.html` (How it works) and `studio.html` (the Studio). Keep both files in the root so the toggle keeps working.

1. **Add file → Upload files** in this repository.
2. Drag in the changed file or files — the same filename replaces the old one.
3. Commit changes.
4. GitHub Pages rebuilds automatically — the Actions tab shows a green tick when it's live (usually under a minute). The URL stays the same.
5. Hard refresh (Ctrl/Cmd + Shift + R) to clear the cache.

## Contact

SMEDTEC Ltd — medical device & consumer-health regulatory consultancy

Sherif Elkhadem, Director · [info@smedtec.co.uk](mailto:info@smedtec.co.uk) · smedtec.co.uk

© 2026 SMEDTEC Ltd. All rights reserved.
