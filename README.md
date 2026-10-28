# Online OCR backend

Deploy this folder to a Node.js host. Set:
- `GEMINI_API_KEY` = your Gemini API key (server-side secret)
- optional `GEMINI_MODEL` = a model available to your account
- `PORT` is normally supplied by the host

Start command: `npm start`

The app expects an HTTPS URL for the deployed service. Protect this endpoint with rate limits/authentication before public production use, because an unprotected endpoint can incur API costs. Images are sent to the online model for recognition; do not upload sensitive documents unless you are comfortable with the provider's data handling terms.
