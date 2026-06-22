Contributing to Dojo Ascension 🥋

Welcome, Co-Architect.

In the spirit of Solarpunk ideals and open-source cooperation, this Dojo relies on the community to build its curriculum. You do not need to be a master Python programmer to contribute! Because our curriculum is data-driven, educators, writers, genealogists, and domain experts can add entirely new lessons just by editing a JSON file.

The Core Philosophy

Code is more than syntax; it is digital ecology. When contributing a mission, we ask that you connect the technical concept to broader human systems:

Philosophy / Martial Arts: How does this relate to discipline, resilience, or human action?

Economics / Governance: How does this relate to resource management, infrastructure, or community organization?

How to Add a Mission

All missions live in missions.json. To add a new mission, you simply add a new JSON object to the array.

The Mission Schema

Please adhere strictly to this schema to ensure the Dojo Engine parses your mission correctly.

{
    "id": "unique_stable_identifier",
    "number": 11,
    "title": "Your Mission Title",
    "philosophy": "A cross-disciplinary analogy (e.g., Theatre, Martial Arts).",
    "economics": "An economic or governance analogy (e.g., Supply chains, Baltic e-governance).",
    "tech_concept": "The actual technical explanation of the code.",
    "challenge": "The prompt asking the user to write code.",
    "answer": ["list", "of", "acceptable", "answers"],
    "skill_target": "domain"
}


Schema Rules

id: Must be a stable string (e.g., "git_branching_merging"). Do not rely on number as it may change if missions are reordered.

answer: MUST BE AN ARRAY [ ]. This allows you to accept multiple valid user inputs (e.g., ["seed = 42", "seed=42"]).

skill_target: The core competency this mission trains. Current supported domains: python, git, json, architecture, review.

Journalistic Integrity & AI Transparency

As a project that values transparency and verifiable works, we treat code contributions like journalistic sources.

If you used an AI (like GitHub Copilot, Gemini, or ChatGPT) to help draft your mission's JSON, code, or philosophical analogies, we encourage you to cite your AI partner. * When submitting your Pull Request (PR), simply include a link to your shared AI chat (e.g., a Copilot Share link) or paste the prompt you used.

This allows the community to review the "genealogy" of the thought process and ensures our tools remain transparent sparring partners rather than black-box oracles.

Getting Started

Fork the repository.

Branch off of main (git checkout -b feature/new-mission-pack).

Add your mission to missions.json (or propose a new pack like journalism.json).

Test the Dojo locally (python dojo_classroom.py) to ensure the engine loads your JSON.

Push your branch and open a Pull Request.

"Let us never stop learning from Galileo."
