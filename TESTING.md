# Manual Testing

## Local Server Verification
- Start a simple HTTP server: `python -m http.server 8000`
- Request each static page to confirm an HTTP 200 response:
  - `curl -s -o /tmp/index.html -w '%{http_code}\n' http://127.0.0.1:8000/index.html`
  - `curl -s -o /tmp/about.html -w '%{http_code}\n' http://127.0.0.1:8000/about.html`
  - `curl -s -o /tmp/projects.html -w '%{http_code}\n' http://127.0.0.1:8000/projects.html`

## Navigation Order Check
- Open each page in a browser and verify the navigation buttons appear in the order:
  1. Home
  2. Projects
  3. About
  4. Contact

These checks ensure the pages load correctly with the current assets and the navigation layout remains consistent across the site before updating the repository.
