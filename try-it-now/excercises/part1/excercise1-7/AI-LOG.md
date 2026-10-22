## What you ask

Excercise 1.7: A page someone else has to maintain,   The situation : you are leaving this project next week. Someone will take it over, and they will not be able to ask you anything. Everything they need to know has to be in the file.   Build a page for a real audience - a study guide for your class, a page for a club or society you belong to, a set of directions to somewhere people keep getting lost finding.  Requirements: create document-page.html,  At least three sections, a mix of paragraphs and lists, correct heading hierarchy, HTML comments that: Mark each major section, Explain any structure whose reason is not obvious from the code, include at least one <!-- TODO: --> naming a real, specific next step, Properly indented (let Prettier do it -see 0d). Example :  <!-- Header Section -->, <!-- Main Content -->    Comment the why, never the what .    <!-- this is a heading --> above an <h1> is noise; the code already said that. <!-- Ordered by payoff, not alphabetically --> is information that exists nowhere else in the file, and it is the only reason comments exist. A good test: if deleting the comment loses nothing, it was never a comment - it was a translation..

## What you got 

I built `document-page.html` as an information page for Yakar FSE, since you run it. Prettier's check passes on the file.

**What's on the page**
- **Sections:** it has three `<h2>` sections: About the school, How to apply, and What to bring to your first session. Players and coaches each get an `<h3>` under How to apply, and each `<h3>` has a short paragraph and a numbered list.
- **Comments:** each major section has a comment that says why it is built that way, for example why "How to apply" comes right after a short About section, and why the steps are an `<ol>` and the kit list a `<ul>`. A note in the head explains the rule for the whole file: only confirmed facts go on the page, and gaps become TODOs. The CSS comments record the system-fonts choice and the contrast ratios for the club's red, blue and white.

There are four TODOs, each naming a specific next step:
- Replace the player application link, which is currently `#`.
- Replace the coach application link, also `#`.
- Add a "Training times" section once the timetable is confirmed.
- Add a "Contact" section once a phone or WhatsApp number is confirmed.

The page deliberately has no training times, venue, fees or contact details, because I only had the confirmed facts: the club, the 2026 tournament and Abuko Primary School field. I invented the application steps and the "what to bring" list as plausible football basics, so check them against how the club really works before publishing. Don't publish with the two `#` links, because they only scroll to the top.

## What you have changed 

please help and display the code.