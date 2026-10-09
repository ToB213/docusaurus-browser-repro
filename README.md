# Docusaurus Default Browser Reproduction

Minimal reproduction for an issue where Docusaurus opens
a running Chromium-based browser instead of the system
default browser on macOS.

## Environment

- Docusaurus: 3.10.2
- Node.js: 24.16.0
- macOS: 27.0

## Steps to reproduce

1. Set Firefox as the default browser on macOS.
2. Launch Firefox and Google Chrome.
3. Install dependencies using `npm install`.
4. Run `npm run start`.
5. Observe that Chrome opens instead of Firefox.
6. Stop the development server and quit Chrome.
7. Run `npm run start` again.
8. Observe that Firefox opens.

## Expected behavior

Docusaurus should respect the system default browser
unless another browser is explicitly specified.
