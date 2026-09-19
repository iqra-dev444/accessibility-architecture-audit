# Accessibility Baseline Audit

## Audit Overview

A baseline accessibility audit was performed on the India Post public-facing website using:

- Google Lighthouse
- Keyboard-only navigation

The audit focused on identifying accessibility and related usability issues and documenting evidence, user impact, severity, and recommended remediation.

## Audit Findings

### WEB-001 — Links Without a Discernible Name

**Page/Component:** Homepage

**WCAG Reference:** WCAG 2.4.4 — Link Purpose

**Evidence:**  
Lighthouse reported that links do not have a discernible name, including an `a.undefined` element.

**Severity/Priority:** Moderate

**User Impact:**  
Screen-reader users may not be able to understand the purpose or destination of the affected link.

**Recommended Fix:**  
Provide every link with a clear and accessible name that describes its purpose or destination.

**Status:** Open

---

### WEB-002 — Insufficient Color Contrast

**Page/Component:** Homepage

**WCAG Reference:** WCAG 1.4.3 — Contrast (Minimum)

**Evidence:**  
Lighthouse reported that background and foreground colors do not have a sufficient contrast ratio.

**Severity/Priority:** Moderate

**User Impact:**  
Users may have difficulty reading text when there is insufficient contrast between the foreground and background colors.

**Recommended Fix:**  
Increase the contrast ratio between foreground text and its background so that the content is easier to read.

**Status:** Open

---

### WEB-003 — Heading Elements Not in Sequential Order

**Page/Component:** Homepage

**WCAG Reference:** WCAG 2.4.6 — Headings and Labels

**Evidence:**  
Lighthouse reported that heading elements are not in a sequentially descending order, including an `h5` heading.

**Severity/Priority:** Moderate

**User Impact:**  
Users of assistive technologies may have difficulty understanding the structure and hierarchy of the page.

**Recommended Fix:**  
Use a logical heading hierarchy and ensure heading levels follow the appropriate document structure.

**Status:** Open

---

### WEB-004 — Touch Targets With Insufficient Size or Spacing

**Page/Component:** Homepage

**WCAG Reference:** Best Practices

**Evidence:**  
Lighthouse reported that touch targets do not have sufficient size or spacing.

**Severity/Priority:** Moderate

**User Impact:**  
Users may have difficulty activating controls accurately on touch devices, particularly when interactive elements are small or positioned too close together.

**Recommended Fix:**  
Increase the size and spacing of interactive touch targets to make them easier to select.

**Status:** Open

---

### WEB-005 — Third-Party Cookies Detected

**Page/Component:** Homepage

**WCAG Reference:** Best Practices

**Evidence:**  
Lighthouse reported the use of third-party cookies, with 34 cookies detected.

**Severity/Priority:** Low

**User Impact:**  
Third-party cookies may be blocked by browsers and can have privacy and compatibility implications.

**Recommended Fix:**  
Review whether each third-party cookie is necessary and consider privacy-preserving alternatives where appropriate.

**Status:** Open

---

## Keyboard Navigation Review

A keyboard-only navigation pass was performed using the `Tab` and `Shift + Tab` keys.

The tested controls displayed visible keyboard focus indicators, allowing navigation between interactive elements using the keyboard.

A screenshot of the keyboard navigation test is included in the `docs` directory.

## Evidence

Supporting screenshots from the audit are stored in the `docs` directory:

- `lighthouse-accessibility.png`
- `lighthouse-best-practices.png`
- `keyboard-navigation.png`

## Audit Summary

The audit identified five issues requiring attention:

1. Links without a discernible name
2. Insufficient color contrast
3. Heading elements not in sequential order
4. Touch targets with insufficient size or spacing
5. Third-party cookies detected on the homepage

The findings provide a baseline for improving accessibility, usability, and maintainability of the project.

## Remediation Priority

The findings are prioritized according to their potential impact on users:

- **Moderate:** WEB-001, WEB-002, WEB-003, WEB-004
- **Low:** WEB-005

All findings are currently marked as **Open** and can be addressed during future implementation work.
