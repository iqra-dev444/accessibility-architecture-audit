# Repository Architecture

## Project Structure

This repository follows a monorepo-style structure.

- `client/` - Frontend application code
- `server/` - Backend application code
- `docs/` - Accessibility audit and project documentation
- `tests/` - Testing resources

## Architecture Boundaries

### Client
Contains the frontend user interface and client-side application code.

### Server
Contains backend services and server-side application code.

### Docs
Contains accessibility audit findings, evidence, and architecture documentation.

### Tests
Contains automated and manual testing resources.

## Local Setup

The repository is organized into separate directories for the frontend, backend, documentation, and tests. This structure allows each part of the project to be developed and maintained independently.

## First Vertical Feature Slice

The first vertical feature slice will connect a frontend interface with the corresponding server functionality and testing resources. Supporting documentation will be maintained in the `docs` directory.

## Accessibility Audit

The accessibility baseline was reviewed using Lighthouse and keyboard-only navigation.

The documented findings include:

1. Links without a discernible name
2. Insufficient color contrast
3. Heading elements not in sequential order
4. Touch targets with insufficient size or spacing
5. Third-party cookies detected on the homepage

Detailed findings are documented in `ACCESSIBILITY-AUDIT.md`.
