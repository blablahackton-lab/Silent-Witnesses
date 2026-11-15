# Abandoned but Not Forgotten

> **The Machines We Left Behind.** An independent, educational archive of the robotic spacecraft humanity has left on the Moon, on Mars, in Earth orbit, and in deep space.

**NASA Space Apps Challenge 2026 Submission**  
- **Challenge:** Abandoned but Not Forgotten  
- **Team:** The feed bats  
- **Event:** Registered for the local event in Itahari, Nepal; participated virtually  
- **Repository:** [https://github.com/blablahackton-lab/Silent-Witnesses](https://github.com/blablahackton-lab/Silent-Witnesses)  
- **Live Demo:** [https://silent-witnesses.onrender.com/](https://silent-witnesses.onrender.com/)

---

> [!NOTE]  
> **Disclaimer:** This is an independent educational project created for a hackathon. It is not affiliated with, endorsed by, or sponsored by NASA. Mission facts are summarized from public NASA sources, linked throughout the site.

---

## Table of Contents
- [The Idea](#the-idea)
- [Challenge and How We Addressed It](#challenge-and-how-we-addressed-it)
- [Features](#features)
- [What's in the Archive](#whats-in-the-archive)
- [Tech Stack](#tech-stack)
- [Data and Sources](#data-and-sources)
- [Accuracy Principles](#accuracy-principles)
- [Use of AI](#use-of-ai)
- [Team](#team)
- [Acknowledgements](#acknowledgements)
- [License](#license)

---

## The Idea
For more than 60 years, humanity has sent machines far beyond Earth. Many finished their jobs and went quiet. Some still work. Some were lost. A few are still sending data from beyond the Sun's protective bubble.

**Abandoned but Not Forgotten** tells their stories in one place. You can browse landers, rovers, orbiters, satellites, and flyby spacecraft, see what each one did, and find out what happened to it: active, extended mission, completed, inactive, lost communication, or unknown.

Where a spacecraft's fate or location is uncertain, we state it clearly instead of guessing.

---

## Challenge and How We Addressed It

### Challenge
**Abandoned but Not Forgotten**

### Problem
Information about past and present space missions is scattered across different archives, and the status of older hardware is easy to get wrong or oversimplify.

### Our Solution
A single, searchable, mobile-friendly archive that groups missions by destination, labels each mission's status honestly, and links back to NASA references for every claim.

### Audience
Students, educators, space enthusiasts, and curious members of the public.

---

## Features
- **Interactive 3D Hero:** A WebGL scene (Three.js) built from an embedded 3D model, plus procedurally generated Earth and Moon surfaces.
- **Four Destination Pages:** Moon, Mars, Earth Orbit, and Deep Space, each featuring an intro and a chronological mission log.
- **Searchable Mission Archive:** Search by name and filter by destination, decade, mission type, and status.
- **Dedicated Voyager 1 & 2 Section:** Mission overview, engineering details, planetary encounters, the Golden Record, Pale Blue Dot, interstellar crossings, a detailed mission timeline, and a side-by-side comparison table.
- **Rover & Lander Comparison Table:** Detailed metrics for Sojourner, Spirit, Opportunity, Curiosity, and Perseverance.
- **Status Badges:** Color-coded status labels (*Active*, *Extended mission*, *Completed*, *Inactive*, *Lost*, *Unknown*).
- **Source Links on Every Mission:** Each entry references official NASA documentation.
- **Accessible by Design:** Skip link, keyboard focus styles, semantic HTML landmarks, and `prefers-reduced-motion` support.
- **Responsive & Self-Contained:** Fully responsive UI with mobile menu drawer and safe-area support.

---

## What's in the Archive
40 missions across four destinations:

| Destination | Mission Examples |
| :--- | :--- |
| 🌑 **Moon** | Ranger 7–9, Lunar Orbiter, Surveyor, Apollo Lunar Module descent stages, Lunar Roving Vehicle, ALSEP stations |
| 🔴 **Mars** | Mariner 4/6/7/9, Viking 1 and 2, Pathfinder and Sojourner, Spirit, Opportunity, Phoenix, Curiosity, InSight, Perseverance, Ingenuity, Odyssey, MRO, MAVEN |
| 🌍 **Earth Orbit** | TIROS-1, Nimbus, Landsat, Seasat, Hubble, Chandra, Terra and Aqua, Envisat (non-NASA, labelled) |
| 🚀 **Deep Space** | Pioneer 10 and 11, Voyager 1 and 2, Galileo, Ulysses, Cassini–Huygens, New Horizons |

---

## Tech Stack
- **Languages:** HTML5, CSS3, vanilla modern JavaScript (no framework, zero build tools).
- **3D Graphics:** [Three.js r128](https://threejs.org/) & `GLTFLoader` (via CDN).
- **Routing:** Hash-based client-side routing (`#moon`, `#mars`, `#archive`, `#voyager`).
- **Data Architecture:** In-memory, data-driven architecture where missions live in a structured JavaScript data store powering all dynamic views and filters.
- **Typography:** Instrument Sans, Newsreader, and Big Shoulders Display via Google Fonts.
- **Deployment:** Dockerized lightweight Nginx hosted on Render.

---

## Data and Sources
All content is summarized in our own words from public NASA material:
- [NASA Science](https://science.nasa.gov/)
- [NASA Mars Exploration](https://science.nasa.gov/mars/)
- [NASA Voyager Mission](https://science.nasa.gov/mission/voyager/)
- [Where are Voyager 1 and Voyager 2 now?](https://science.nasa.gov/mission/voyager/where-are-voyager-1-and-voyager-2-now/)
- [NASA History: Human Artifacts on the Moon](https://www.nasa.gov/wp-content/uploads/static/history/humanartifacts.html)
- [NASA / JPL](https://www.jpl.nasa.gov/)

*Note: Mission status and instrument details can change. The Voyager data was verified against NASA reporting on 15 November 2026 and links to NASA's live status page for real-time telemetry.*

---

## Accuracy Principles
1. **Say what we know:** If a location or fate is uncertain (for example, some Apollo ascent stages), the site explicitly notes it.
2. **Don't mislabel:** Orbiters are labelled as orbiters, and only landers and rovers are described as resting on surfaces.
3. **Inactive isn't abandoned:** An inactive satellite is not automatically uncontrolled or lost.
4. **Credit the source:** Non-NASA missions (such as ESA's Envisat) are clearly attributed, and every entry links to an authoritative source.

---

## Use of AI
We used AI tools as assistants while building this project. The team made all architectural decisions, chose the structure and topics, and reviewed all output.

- **Tools used:** Claude, Codex, and Gemini.
- **Purpose:** Drafting copy, generating boilerplate code, debugging, and brainstorming.
- **Fact-checking:** Mission facts (dates, statuses, locations, and instrument details) were verified against public NASA sources listed in [Data and Sources](#data-and-sources).
- **Limits:** AI-generated text was rigorously checked for hallucinations and outdated mission states.

---

## Team

| Name | Role |
| :--- | :--- |
| **Avinash** | Data Research (Mission Data & NASA Sources) |
| **Abhyuday** | Developer |
| **Ubik** | Developer |

---

## Acknowledgements
- NASA, JPL, ESA, and the mission teams for publishing open space data.
- NASA Space Apps Challenge organizers, mentors, and volunteers.
- [Three.js](https://threejs.org/) community and contributors.
- Everyone who designed, built, and operated the machines chronicled in this project.

---

## License
Code is released under the [MIT License](LICENSE). Mission facts and media descriptions are summarized from public NASA sources. NASA names and insignia are the property of NASA and are used strictly for educational identification and attribution.
