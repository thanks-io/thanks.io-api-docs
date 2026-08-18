# thanks.io API documentation

The Mintlify site behind [docs.thanks.io](https://docs.thanks.io): the public API
reference and the product changelog (`updates.mdx`).

## This repository is public

Everything committed here is world-readable the moment it exists, draft pull
requests included — page content, branch names, commit messages, PR titles and
bodies all count.

Write only what a customer needs in order to use the API. Nothing else belongs
here:

- How the service is built, hosted, or operated.
- Anything that has not shipped to customers yet.
- Anything that identifies people, tickets, costs, or commercial terms.
- Credentials, keys, tokens, or any URL that is not publicly reachable.

If you are unsure whether a detail is already public, check whether it appears
somewhere on docs.thanks.io today. If it doesn't, leave it out.

## Accuracy

- **Never guess, invent, or infer behavior.** If you can't confirm how something
  works, say so and ask — don't write a plausible-sounding description. A wrong
  example in an API reference costs a customer a broken integration.
- Ask for clarification rather than assuming. Cite what you based a change on.
- Push back when an instruction would make the docs worse, and explain why.
  Better documentation is the goal, not agreement.

## Project shape

- MDX files with YAML frontmatter, rendered with Mintlify components.
- `docs.json` owns navigation, theme, and settings — see the
  [docs.json schema](https://mintlify.com/docs.json).

## Frontmatter

Every page needs both, and neither is boilerplate:

- `title` — clear and descriptive. What the page is, in the reader's words.
- `description` — a concise summary. It carries the page in search results and
  in navigation, so write it for someone who hasn't opened the page yet.

Never ship an MDX file without frontmatter.

## Content

- Document just enough for the reader to succeed — not too much, not too little.
- Prefer evergreen phrasing over anything that dates quickly.
- Search for existing coverage before adding a page; don't duplicate.
- Check existing patterns and match the style and formatting of neighbouring
  pages.
- Cover both basic and advanced use cases.
- Second-person voice ("you"). Prerequisites at the start of procedural content.
- Make the smallest reasonable change.

## Code, links, and images

- **Test every code example before publishing it.** Untested examples don't ship.
- Language tag on every code block.
- Alt text on every image.
- Relative paths for internal links — never absolute URLs.

## Before opening a pull request

Run `mint broken-links` and fix everything it reports.

Make the edits and report what changed — you don't stage or commit.
