# Process notes

**Purpose:** a small artifact for the "AI-driven product management — prototype via GitHub connect" checklist item, built to also stand on its own as a real product idea.

**How it was built:**

1. GitHub read access was already verified in the Claude session against the RealPage org connector.
2. This repo was created under the personal GitHub account (`shannagerhart/sspbi-ask-a-measure-prototype`) and made **public**, to avoid the private-repo sign-in issue hit on the first prototype (`sspbi-data-pane-prototype`).
3. Claude generated a small HTML/CSS/JS prototype (`index.html`): a text input plus a keyword-matching rule set that maps a handful of common CRE BI questions (NOI variance, occupancy, recoveries, rent, returns) to an illustrative SSPBI measure and its DAX.
4. Files were committed directly through the GitHub connector (`push_files`) in one commit.

**What this is not:** not a live language model, not connected to the production measure store or the real ~2,317-measure set, not reviewed/approved — a proof-of-concept for the check, and a starting sketch of a real idea.

**If this concept is worth pursuing for real:**

- Swap the keyword rule set for an actual LLM call scoped to the real measure catalog (name + description + DAX per measure), so it generalizes past the five hardcoded question types here.
- Add a feedback loop (thumbs up/down on a suggested measure) to catch bad matches.
- Decide where it would live — inside SSPBI itself, or as a companion Excel Connector feature.
