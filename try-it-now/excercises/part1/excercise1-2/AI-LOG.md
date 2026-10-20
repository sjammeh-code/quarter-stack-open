## What you asked
building a page from an outline, you are writing the page that explains an officials process to people who do not know it- opening a bank account. Requirements : how-to.html, one <h1>: the process being explained, atleast three <h2> sections -  a sensible set is Before you go, What to bring, At the Office, After atleast two <h3> subsections under one of the <h2> s, no skipped levels anywhere, a short paragraph under every heading - real information, not placeholder text, zero validator errors

## What you got
I rewrote `how-to.html` to meet your requirements. A script I ran on it confirmed the heading order and that a paragraph follows every heading. I didn't run it through the W3C validator, so a final check there is worth doing.

- **One h1:** "How to open a bank account".
- **Four h2 sections:** Before you go, What to bring, At the office, and After you open the account.
- **h3 subsections:** two under Before you go (Choose a bank, Choose an account type) and three under At the office (Fill in the application form, Wait for verification, Make your first deposit).
- **No skipped levels:** every h3 sits under an h2, and every h2 sits under the h1.
- **A paragraph under every heading:** each one has real guidance, with no placeholder text.

The markup is plain HTML5 with no unclosed tags, and I escaped the ampersand in the font link so that URL doesn't trigger an error.

I removed the FAQ and glossary from the first version. They would have added headings that needed their own paragraphs and pushed the page past your outline. I can add them back as h3s under After if you want them.

## What you changed and why
please show the code, because it did not give me and code that i can use. i did not do any changes on the code i got.