# User Stories - ADHD Demystified

## MUST (Critical for launch)

1. Title: Clear homepage purpose

Story: As a Visitor, I want the homepage to communicate the site's purpose within 10 seconds so that I can decide whether it's relevant to me.

**Acceptance Criteria:**

- Given I land on the homepage, When I scan the hero, I can see a quick view of what the website is about and services provided.
- find at least one next action (e.g. "Start screener" or "Get help")
- read hero text with sufficient contrast and font size for accessibility

**Tasks:**

- [x] Create hero layout (desktop and mobile) with visual hierarchy.
- [x] Create buttons / links to next actions to allow users to get to relevant sections.

2. Title: Informational symptom & education cards

Story: As an Explorer user, I want easily browsable informational cards about symptoms and ADHD types so that I can learn, compare, and decide which next steps are relevant to me.

Acceptance Criteria:

- Given I click the primary CTA or Diagnosis CTA, When I open the section, Then I can browse a set of informational cards that describe common symptoms, examples, and which ADHD types they commonly relate to.
- Given I view a card, When I can hover it when on a desktop to highlight it so I can focus on each individual card
- Given the user browses cards, When content is displayed, Then the page clearly states these are informational resources and not clinical diagnoses.

Tasks:

- [x] Design card layout with title, short description, tags (symptom/type).
- [x] Populate an initial set of cards covering core symptoms and ADHD types with links to resources.
- [x] Create hover behaviours for user interactivity
- [x] Ensure cards are accessible and readable on mobile readable text sizes.

3. Title: Diagnosis information flow (informational links)

Story: As a Concerned adult/Parent, I want a clear informational flow with links so that I can learn how to get a diagnosis and take practical next steps.

Acceptance Criteria:

- Given I open the Diagnosis section, When I follow the flow, Then each step provides a short explanation and links to trusted resources (GP advice, referral tips, clinician finders).
- Given I read the flow, When I'm preparing for assessment, Then I can find actionable, privacy-aware advice (what to bring, what to expect) and contact options.

Tasks:

- [x] Draft the diagnosis flow content: steps, short explanations, and resource links.
- [x] Add inline links to trusted sources (NHS/ADHD UK) and local signposting where possible.
- [x] Ensure the flow is presented accessibly (clear headings, readable steps, printer-friendly if needed).

4. Title: Mobile usability

Story: As a Mobile user, I want readable text and large tappable targets so that I can use the site comfortably on my phone.

Acceptance Criteria:

- Given a mobile device, When I interact with controls, Then touch targets meet WCAG-friendly sizes and body text is at readable.

Tasks:

- [x] Audit mobile styles and adjust paddings/margins for tappable targets.
- [x] Ensure body font size and scaled sizes meet legibility guidelines.

5. Title: Keyboard & screen-reader navigation

Story: As an Accessibility-focused user, I want keyboard- and screen-reader-friendly tabs and navigation so that I can fully access content.

Acceptance Criteria:

- Given keyboard or screen reader use, When navigating, Then ARIA roles and keyboard interactions are implemented and focus states are visible.
- Given forms, When errors or success occur, Then messages are announced via `aria-live`.

Tasks:

- [x] Add ARIA roles and keyboard handlers for accordion/tabs.
- [x] Ensure visible focus styles and regions for form feedback.

6. Title: Privacy-first contact form

Story: As a Contact form user, I want a simple, privacy-respecting contact form so that I can ask a question without oversharing.

Acceptance Criteria:

- Given I fill the form, When I submit, Then the form requires only necessary fields, shows a short privacy note/consent, and returns success or field-specific error messages.

Tasks:

- [x] Limit form fields to essentials and mark optional fields explicitly.
- [x] success page redirect (`success.html`).

## SHOULD (High value, next iteration)

7. Title: Resource accordion

Story: As a Resource seeker, I want a resource accordion with short summaries so that I can expand items to read details and find trusted sources quickly.

Acceptance Criteria:

- Given I browse Resources, When I view the accordion, Then each collapsed item shows a title and expanding it reveals details, audience tags, and last-reviewed date.
- Given an expanded item, When I need more, Then links to the original source and supports are available.

Tasks:

- [x] Design accordion structure with clear collapsed summaries and expanded detail sections.
- [x] Populate initial accordion items with title, summary and resource links.

8. Title: Header anchor links

Story: As a Visitor, I want quick anchor links in the header so that I can jump to relevant sections without scrolling.

Acceptance Criteria:

- Given header menu use, When I click an anchor, Then the page smoothly scrolls to the section.

Tasks:

- [x] Add anchor links in the header and smooth scroll behavior.

10. Title: Shareable resource links

Story: As a Clinician/Advocate, I want shareable resource links so that I can easily recommend specific items to others.

Acceptance Criteria:

- Given a resource card, When I copy the URL, Then a stable link or is provided.

Tasks:

- [ ] Ensure each resource has a stable anchor or permalink.

## COULD (Nice-to-have)

12. Title: Resource filters by audience

Story: As a Resource browser, I could filter resources by audience (Adults, Teens, Parents) so that I find relevant materials faster.

Acceptance Criteria:

- Given filters, When a filter is selected, Then resource cards update to show matching items.

Tasks:

- [ ] Add filter UI and client-side filtering logic.
- [ ] Add audience metadata to resource items.

## WON'T (Out of scope for initial launch)

14. Diagnostic assessments online (explicit WON'T)

Story: As a User, I will not be able to complete a clinical diagnostic assessment online; the site provides guidance and signposting only.

- Rationale: Diagnostic decisions require clinical engagement; site is informational and signposting only.
