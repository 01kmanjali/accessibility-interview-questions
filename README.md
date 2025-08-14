# ARIA & Accessibility Interview Questions & Answers

### This document contains common ARIA and accessibility-related interview questions with detailed answers, examples, and best practices.

---

## Table of Contents

<details open>
  <summary>Show Table of Contents</summary>

  | No.  | Questions                                                                                                                                                                                                                                                                               |
  | -- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
  | 1  | [Who benefits from accessibility?](#1-who-benefits-from-accessibility)                                                                                                                                                                                                                  |
  | 2  | [How would you define inclusive and/or universal design?](#2-how-would-you-define-inclusive-andor-universal-design)                                                                                                                                                                     |
  | 3  | [How has your approach to accessibility changed over time?](#3-how-has-your-approach-to-accessibility-changed-over-time)                                                                                                                                                                |
  | 4  | [Name some ways responsive/mobile-first design can affect accessibility.](#4-name-some-ways-responsivemobile-first-design-can-affect-accessibility)                                                                                                                                     |
  | 5  | [What are some UX concerns with iconography in UI?](#5-what-are-some-ux-concerns-with-iconography-in-ui)                                                                                                                                                                                |
  | 6  | [What assistive technologies (ATs) are you familiar with?](#6-what-assistive-technologies-ats-are-you-familiar-with)                                                                                                                                                                    |
  | 7  | [Purpose of heading and header elements](#7-purpose-of-heading-and-header-elements)                                                                                                                                                                                                     |
  | 8  | [What are skip links?](#8-what-are-skip-links)                                                                                                                                                                                                                                          |
  | 9  | [Tools to test accessibility](#9-tools-to-test-accessibility)                                                                                                                                                                                                                           |
  | 10 | [How can plain language benefit accessibility?](#10-how-can-plain-language-benefit-accessibility)                                                                                                                                                                                       |
  | 11 | [Appropriate use of link, generic button, and submit button](#11-appropriate-use-of-link-generic-button-and-submit-button)                                                                                                                                                              |
  | 12 | [Ways to indicate an element or component’s state](#12-ways-to-indicate-an-element-or-components-state)                                                                                                                                                                                 |
  | 13 | [How can carousels be problematic for users with disabilities?](#13-how-can-carousels-be-problematic-for-users-with-disabilities)                                                                                                                                                       |
  | 14 | [Design considerations for supporting text resize/zoom](#14-design-considerations-for-supporting-text-resizezoom)                                                                                                                                                                       |
  | 15 | [In what ways can the CSS `display` property affect the accessibility of a document?](#15-in-what-ways-can-the-css-display-property-affect-the-accessibility-of-a-document)                                                                                                             |
  | 16 | [What is the difference between `legend` and `label` elements?](#16-what-is-the-difference-between-legend-and-label-elements)                                                                                                                                                           |
  | 17 | [What is the purpose of the `alt` attribute for images?](#17-what-is-the-purpose-of-the-alt-attribute-for-images)                                                                                                                                                                       |
  | —  | [Effect of an empty `alt` or missing attribute](#effect-of-an-empty-alt-or-missing-attribute)                                                                                                                                                                                           |
  | —  | [Appropriate instances for empty or missing `alt`](#appropriate-instances-for-empty-or-missing-alt)                                                                                                                                                                                     |
  | —  | [Context-based alternative text](#context-based-alternative-text)                                                                                                                                                                                                                       |
  | —  | [Providing alternative text for SVGs](#providing-alternative-text-for-svgs)                                                                                                                                                                                                             |
  | 18 | [What methods would you use to find an element’s accessible name?](#18-what-methods-would-you-use-to-find-an-elements-accessible-name)                                                                                                                                                  |
  | 19 | [What is the accessibility tree?](#19-what-is-the-accessibility-tree)                                                                                                                                                                                                                   |
  | 20 | [Why are `rems` or `ems` preferable to pixels for setting type size?](#20-why-are-rems-or-ems-preferable-to-pixels-for-setting-type-size)                                                                                                                                               |
  | 21 | [Why is it important to allow the viewport to scale?](#21-why-is-it-important-to-allow-the-viewport-to-scale)                                                                                                                                                                           |
  | 22 | [How is the `title` attribute exposed to assistive technologies?](#22-how-is-the-title-attribute-exposed-to-assistive-technologies)                                                                                                                                                     |
  | —  | [Elements that can use `title`](#elements-that-can-use-title)                                                                                                                                                                                                                           |
  | —  | [Appropriate use of `title`](#appropriate-use-of-title)                                                                                                                                                                                                                                 |
  | 23 | [Describe a scenario where you might need to use aria-describedby](#23-describe-a-scenario-where-you-might-need-to-use-aria-describedby)                                                                                                                                                |
  | 24 | [What are landmark roles and how can they be useful?](#24-what-are-landmark-roles-and-how-can-they-be-useful)                                                                                                                                                                           |
  | 25 | [When to use a toggle button, a switch control, or a checkbox?](#25-when-to-use-a-toggle-button-a-switch-control-or-a-checkbox)                                                                                                                                                         |
  | 26 | [Methods to hide content](#26-methods-to-hide-content)                                                                                                                                                                                                                                  |
  | 27 | [Is it possible to overuse ARIA?](#27-is-it-possible-to-overuse-aria)                                                                                                                                                                                                                   |
  | 28 | [Assistive technologies affected by ARIA](#28-assistive-technologies-affected-by-aria)                                                                                                                                                                                                  |
  | 29 | [Difference between hidden, aria-hidden="true", and role="presentation"/"none"](#29-difference-between-hidden-aria-hiddentrue-and-rolepresentationnone)                                                                                                                                 |
  | 30 | [When to use aria-live and possible values](#30-when-to-use-aria-live-and-possible-values)                                                                                                                                                                                              |
  | 31 | [Marking up a decorative icon font or SVG](#31-marking-up-a-decorative-icon-font-or-svg)                                                                                                                                                                                                |
  | 32 | [How screen readers treat CSS pseudo content](#32-how-screen-readers-treat-css-pseudo-content)                                                                                                                                                                                          |
  | 33 | [Describe the steps you take in reviewing or auditing a website or application for accessibility](#33-describe-the-steps-you-take-in-reviewing-or-auditing-a-website-or-application-for-accessibility)                                                                                  |
  | 34 | [Describe an instance where an automated test would not flag a blatant accessibility error](#34-describe-an-instance-where-an-automated-test-would-not-flag-a-blatant-accessibility-error)                                                                                              |
  | 35 | [When should you use or recommend ARIA roles or attributes to solve an accessibility issue?](#35-when-should-you-use-or-recommend-aria-roles-or-attributes-to-solve-an-accessibility-issue)                                                                                             |
  | 36 | [Describe your process for figuring out if an accessibility bug is due to a developer, browser, or assistive technology error](#36-describe-your-process-for-figuring-out-if-an-accessibility-bug-is-due-to-a-developer-browser-or-assistive-technology-error)                          |
  | 37 | [Describe your thoughts on how a single page web app should handle focus when a new screen loads](#37-describe-your-thoughts-on-how-a-single-page-web-app-should-handle-focus-when-a-new-screen-loads)                                                                                  |
  | 38 | [Name an ARIA attribute that requires either a child/parent relationship or a pairing role](#38-name-an-aria-attribute-that-requires-either-a-childparent-relationship-or-a-pairing-role)                                                                                               |
  | 39 | [What is your understanding of “accessible name computation” and how it affects modifying the way screen readers announce certain content?](#39-what-is-your-understanding-of-accessible-name-computation-and-how-it-affects-modifying-the-way-screen-readers-announce-certain-content) |
  | 40 | [What are some issues with modifying normal scrolling behavior?](#40-what-are-some-issues-with-modifying-normal-scrolling-behavior)                                                                                                                                                     |
</details>

***
# Accessibility in Design

<details open>
  <summary>Show Table of Contents</summary>

  | No. | Question                                                                                                                            |
  | - | ----------------------------------------------------------------------------------------------------------------------------------- |
  | 1 | [Pros and Cons of Flat vs Skeuomorphic Design for Accessibility](#1-pros-and-cons-of-flat-vs-skeuomorphic-design-for-accessibility) |
  | 2 | [Importance of Color Contrast in Inclusive Design](#2-importance-of-color-contrast-in-inclusive-design)                             |
  | 3 | [States of Actionable Elements Beyond :hover](#3-states-of-actionable-elements-beyond-hover)                                        |
  | 4 | [When to Remove Visual Outline from Focused Elements](#4-when-to-remove-visual-outline-from-focused-elements)                       |
  | 5 | [Placement of Error Messages in Forms](#5-placement-of-error-messages-in-forms)                                                     |
  | 6 | [Impact of Animation on User Experience](#6-impact-of-animation-on-user-experience)                                                 |
  | 7 | [Making Infographics Accessible for Screen Readers](#7-making-infographics-accessible-for-screen-readers)                           |
  | 8 | [Why Color Alone is Insufficient to Convey State](#8-why-color-alone-is-insufficient-to-convey-state)                               |
</details>

***

## 1 Who benefits from accessibility?

* **Primary beneficiaries**: People with disabilities (visual, auditory, cognitive, motor, and speech impairments).
* **Secondary beneficiaries**: Elderly users, people with temporary injuries, low-bandwidth users, and mobile users in challenging environments.
* **Example**: Closed captions help people with hearing loss, but also benefit users in noisy public spaces.

***

## 2. How would you define inclusive and/or universal design?

* **Inclusive Design**: Designing products and experiences usable by as many people as possible, regardless of their abilities or backgrounds.
* **Universal Design**: A broader concept ensuring that the design is inherently accessible without needing adaptation.
* **Example**: Ramps alongside stairs benefit wheelchair users, parents with strollers, and delivery workers.

***

## 3. How has your approach to accessibility changed over time?

* **Earlier**: Accessibility was treated as a checklist at the end of development.
* **Now**: Accessibility is embedded from the start — in design, development, and testing.
* **Improvement**: Shifted from "fixing issues" to **designing inclusively** from the beginning.

***

## 4. Name some ways responsive/mobile-first design can affect accessibility.

* Ensures content adapts to all screen sizes and orientations.
* Improves readability with scalable fonts and touch-friendly targets.
* Avoids horizontal scrolling and ensures elements are not overlapping.
* Helps users with motor impairments by making buttons larger and spaced out.

***

## 5. What are some UX concerns with iconography in UI?

* **Without text labels**, icons can be unclear (e.g., a “gear” could mean settings or tools).
* Icons must have **ARIA labels** or screen-reader text.
* Avoid using color alone to convey meaning — add text or shape differences.

***

## 6. What assistive technologies (ATs) are you familiar with?

* **Desktop**: NVDA, JAWS, VoiceOver, ZoomText.
* **Mobile**: TalkBack (Android), VoiceOver (iOS).
* **Skill level**: Proficient in NVDA, comfortable with VoiceOver and TalkBack.

***

## 7. Purpose of heading and header elements

* **Headings (`<h1>` to `<h6>`)**: Provide document structure for screen readers, improve SEO, and guide navigation.
* **Header landmark (`<header>`)**: Groups introductory content, making it easy for AT users to find context.

***

## 8. What are skip links?

* **Definition**: Links allowing users to skip repetitive navigation and go directly to main content.
* **Benefits**: Saves time for keyboard and screen reader users.
* **Limitations**: If poorly implemented or hidden incorrectly, they may not be discoverable.

***

## 9. Tools to test accessibility

* **Automated**: Axe, Lighthouse, WAVE, Pa11y.
* **Manual**: NVDA, VoiceOver, keyboard-only navigation.
* **Browser Extensions**: Axe DevTools, Accessibility Insights.

***

## 10. How can plain language benefit accessibility?

* Reduces cognitive load for users with reading disabilities or limited literacy.
* Makes content easier for translation and localization.
* Improves comprehension for all users.

***

## 11. Appropriate use of link, generic button, and submit button

* **Link**: Navigates to another page/URL.
* **Generic Button (`<button>`)**: Triggers a client-side action (e.g., opening a modal).
* **Submit Button**: Submits form data to a server.

***

## 12. Ways to indicate an element or component’s state

* Use **ARIA attributes** like:
  * `aria-pressed` (toggle button state)
  * `aria-expanded` (menu open/closed)
  * `aria-disabled` (disabled state)
* Provide **visual cues**: Color changes, icons, animations.
* Ensure **state changes** are announced to screen readers.

***

## 13. How can carousels be problematic for users with disabilities?

* **Auto-advancing slides** can cause motion sickness or disorientation.
* Difficult for keyboard and screen reader users to control.
* Poor focus management can cause navigation issues.
* **Best Practice**: Provide pause/stop controls and accessible navigation buttons.

***

## 14. Design considerations for supporting text resize/zoom

* Use **relative units** (em, rem, %) instead of fixed px values.
* Ensure layouts adapt without breaking when zoomed to 200%+.
* Avoid text being clipped or overlapping when resized.
* **Mobile**: Respect user-set font size preferences via `font-size: 100%` or `1rem`.

***

## 15. In what ways can the CSS `display` property affect the accessibility of a document?

The `display` property can hide content from visual users without necessarily hiding it from assistive technologies, or vice versa. For example:

* `display: none` removes the element from both visual display and the accessibility tree.
* `visibility: hidden` hides it visually but still affects layout.
* Improper use can make interactive elements inaccessible to screen readers.

***

## 16. What is the difference between `legend` and `label` elements?

* **`legend`**: Provides a caption for a `<fieldset>` element, describing a group of related form controls.
* **`label`**: Describes a single form control (like `<input>`, `<textarea>`), associating text with a specific input.

***

## 17. What is the purpose of the `alt` attribute for images?

The `alt` attribute provides alternative text for images, read aloud by screen readers, allowing users who can't see the image to understand its content.

***

### Effect of an empty `alt` or missing attribute

* **Empty`alt` (`alt=""`)**: Screen readers skip the image; used for purely decorative images.
* **No`alt` attribute**: Screen readers may read the image's file name, which is usually unhelpful.

***

### Appropriate instances for empty or missing `alt`

* Empty `alt`: Decorative images that add no meaningful content.
* Missing `alt`: Rarely recommended; might be appropriate in automated content where no description is available.

***

### Context-based alternative text

Alternative text should describe the function or meaning of the image based on its context in the page.

***

### Providing alternative text for SVGs

Use `<title>` or `<desc>` elements inside the SVG for accessibility. Also, use `aria-label` or `aria-labelledby` attributes.

***

## 18. What methods would you use to find an element’s accessible name?

* Use browser dev tools Accessibility panel.
* Check the `aria-label`, `aria-labelledby`, or `<label>` association.
* Use screen reader testing.

***

## 19. What is the accessibility tree?

A structure that assistive technologies use, derived from the DOM, containing only accessible information about elements (name, role, state, value).

***

## 20. Why are `rems` or `ems` preferable to pixels for setting type size?

They scale with user preferences, respecting browser font size settings, improving readability for low-vision users.

***

## 21. Why is it important to allow the viewport to scale?

Preventing zoom (`user-scalable=no`) can make content inaccessible for users with low vision who rely on magnification.

***

## 22. How is the `title` attribute exposed to assistive technologies?

* Some screen readers read the `title` attribute when the element is focused.
* It may appear as a tooltip visually.

***

### Elements that can use `title`

Almost any HTML element.

***

### Appropriate use of `title`

Supplementary information, not essential content, since some users (especially mobile) may never see it.

**Tip:** Always test changes with screen readers and accessibility testing tools to ensure compliance and usability.



***

## 23. Describe a scenario where you might need to use aria-describedby

You might use `aria-describedby` to associate helper text or error messages with a form input so screen reader users get extra context.\
Example: A password input with a note “Must be at least 8 characters.”

***

## 24. What are landmark roles and how can they be useful?

Landmark roles (`banner`, `navigation`, `main`, `complementary`, `contentinfo`) define major sections of a page.\
They help assistive tech users quickly navigate to important areas without reading the entire page.

***

## 25. When to use a toggle button, a switch control, or a checkbox?

* **Toggle button**: For switching between two states in a button UI (e.g., play/pause).
* **Switch control**: Represents an on/off setting, like a light switch in UI.
* **Checkbox**: For selecting multiple independent options.

***

## 26. Methods to hide content

* **From all users**: `display: none;` or `hidden` attribute — removes from accessibility tree and visual UI.
* **From only screen reader users**: `aria-hidden="true"` — visible visually but ignored by assistive tech.
* **From sighted users but not screen readers**: Use off-screen positioning (`position: absolute; left: -9999px;`).
* **Why**: Improves usability, hides decorative or redundant info, or provides accessible-only instructions.

***

## 27. Is it possible to overuse ARIA?

Yes. Adding unnecessary ARIA roles or attributes can confuse assistive technologies, duplicate native semantics, or cause incorrect announcements.

***

## 28. Assistive technologies affected by ARIA

Besides screen readers, ARIA can affect:

* Screen magnifiers
* Voice control software
* Switch devices
* Braille displays\
  ARIA impacts how these tools interpret and present UI elements.

***

## 29. Difference between hidden, aria-hidden="true", and role="presentation"/"none"

* **hidden**: Hides from both visual and accessibility tree.
* **aria-hidden="true"**: Keeps visually but removes from accessibility tree.
* **role="presentation"/"none"**: Removes semantic meaning but content may still be read depending on context.

***

## 30. When to use aria-live and possible values

Use `aria-live` to announce dynamic changes without user focus:

* **polite**: For non-urgent updates like “New message received”.
* **assertive**: For urgent updates like “Error: Form submission failed”.

***

## 31. Marking up a decorative icon font or SVG

* Icon font: Use `aria-hidden="true"`.
* SVG: Add `role="img"` only if meaningful, otherwise `aria-hidden="true"` for decorative ones.

***

## 32. How screen readers treat CSS pseudo content

Screen readers generally **ignore** pseudo-elements (`::before`, `::after`) unless they are part of the DOM via accessible name computation. Important info should not be placed solely in pseudo content.

***

### 33. Describe the steps you take in reviewing or auditing a website or application for accessibility

1. Define scope (pages, user flows, devices).
2. Use automated testing tools (e.g., axe, Lighthouse) for initial scan.
3. Conduct manual keyboard navigation testing.
4. Check screen reader compatibility (NVDA, JAWS, VoiceOver).
5. Verify color contrast, font sizes, and responsive behavior.
6. Review semantic HTML and ARIA usage.
7. Document findings with severity levels and recommendations.

***

### 34. Describe an instance where an automated test would not flag a blatant accessibility error

Automated tools might miss incorrect **alt text** (e.g., "image123" instead of a meaningful description) or logical heading structure that visually appears correct but is semantically wrong.

***

### 35. When should you use or recommend ARIA roles or attributes to solve an accessibility issue?

Only when **native HTML semantics** can’t achieve the desired accessibility.\
Example: Using `role="tablist"` and `aria-selected` for a custom tab component.

***

### 36. Describe your process for figuring out if an accessibility bug is due to a developer, browser, or assistive technology error

1. Test in multiple browsers and devices.
2. Compare behavior across different assistive technologies.
3. Review HTML/ARIA implementation.
4. Search known issues in browser/AT bug trackers.
5. Isolate and simplify the test case.

***

### 37. Describe your thoughts on how a single page web app should handle focus when a new screen loads

* Move focus to the main heading or container of the new content.
* Announce the change for screen readers.
* Avoid leaving focus on old, irrelevant elements.

***

### 38. Name an ARIA attribute that requires either a child/parent relationship or a pairing role

* `aria-labelledby` requires a valid element ID to reference.
* `aria-owns` and `aria-controls` require a defined relationship.

***

### 39. What is your understanding of “accessible name computation” and how it affects modifying the way screen readers announce certain content?

Accessible name computation is the process ATs use to determine what to announce for an element.\
It considers `aria-label`, `aria-labelledby`, `alt`, and visible text — in a defined priority.

***

### 40. What are some issues with modifying normal scrolling behavior?

* Infinite scrolling can trap users without a clear end.
* Scrolljacking disrupts expected navigation.
* Can cause motion sickness or disorientation.
* May break screen reader's virtual cursor position.

***

# Accessibility in Design



## 1. Pros and Cons of Flat vs Skeuomorphic Design for Accessibility

**Flat Design**

* **Pros:** Minimal clutter, faster load times, clean interfaces that reduce cognitive load.
* **Cons:** May lack visual cues like shadows and textures that indicate interactivity, making it harder for some users to identify clickable elements.

**Skeuomorphic Design**

* **Pros:** Mimics real-world objects, providing familiar cues for users with low digital literacy.
* **Cons:** Can be visually heavy, cause longer load times, and may overwhelm users with cognitive impairments.

***

## 2. Importance of Color Contrast in Inclusive Design

Good color contrast ensures text and interactive elements are distinguishable for users with low vision or color blindness. WCAG recommends a contrast ratio of:

* **4.5:1** for normal text
* **3:1** for large text

***

## 3. States of Actionable Elements Beyond :hover

Elements like buttons, links, and form fields should have styles for:

* `:focus` – For keyboard navigation
* `:active` – When being clicked or tapped
* `:visited` – For visited links
* `:disabled` – To indicate non-interactive states

These help all users, including those using assistive tech, understand element status.

***

## 4. When to Remove Visual Outline from Focused Elements

Only remove focus outlines if **you replace them with an equally visible custom focus indicator**. Never remove outlines entirely, as this makes keyboard navigation unusable for many.

***

## 5. Placement of Error Messages in Forms

Error messages should be:

* Placed near the relevant field
* Associated with the field using `aria-describedby`
* Summarized at the top of the form for screen readers

***

## 6. Impact of Animation on User Experience

Animations can:

* **Enhance UX**: Guide focus, provide feedback
* **Harm UX**: Trigger motion sickness, distract users with ADHD

Offer a “reduce motion” option via `prefers-reduced-motion` media query.

***

## 7. Making Infographics Accessible for Screen Readers

* Provide a **textual description** or data table alternative
* Use `aria-label` or `aria-describedby` for brief descriptions
* Ensure logical reading order in code

***

## 8. Why Color Alone is Insufficient to Convey State

Color perception varies among users. Always combine color with:

* Text labels
* Icons or patterns
* ARIA states (e.g., `aria-pressed="true"`)

***

**References:**

* [WCAG Guidelines](https://www.w3.org/WAI/WCAG21/quickref/)
* [MDN Web Docs – Accessibility](https://developer.mozilla.org/en-US/docs/Web/Accessibility)

***

**Author:** Anjali\
**Last Updated:** August 2025
