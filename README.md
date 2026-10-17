# Digital Tasbih

A simple digital tasbih for your phone. Upload a photo of your tasbih, tap the button to count, and set a limit to get a congratulations message when you complete it.

## Features

- **Tasbih photo:** upload your own image in the upper half of the screen
- **Tap counter:** one large button at the bottom, one tap equals one count
- **Count limit:** choose 33, 99, 100, 313 or a custom number
- **Milestone message:** a congratulations dialog appears when you reach your limit, then start a new round or keep counting
- **Rounds:** tracks how many rounds you have completed
- **Material You design:** the theme picks up colors from your photo and follows light or dark mode
- **Saved on your device:** count, limit, rounds and photo are kept in your browser
- **Optional vibration** on each tap
- **AI dua reader (optional):** add your own Gemini API key in Settings, upload a screenshot of a dua or dhikr, and the app shows the text and sets the count limit from it (for example, "read this 10 times" sets the limit to 10). You can edit the text and limit afterwards.

## How to use

1. Tap the photo area to upload an image of your tasbih.
2. Tap **Tap to count** to start counting.
3. Tap the gear icon to set a count limit or turn vibration on or off.
4. Tap the reset icon to set the count and rounds back to 0.

## AI setup (optional)

1. Create an API key in [Google AI Studio](https://aistudio.google.com/apikey).
2. Open **Settings** in the app and paste the key. The model name can be changed there if Google retires it.
3. Upload a screenshot of a dua or dhikr.

The key is saved only in your browser, never in the repository. Screenshots are sent to Google for reading. Free-tier limits are set by Google and can change. AI can misread Arabic, so use the edit button to check the text.

## Run locally

No build step or dependencies. Open `index.html` in any modern browser.

## Deploy on GitHub Pages

1. Upload `index.html` to the root of your repository.
2. Go to **Settings → Pages**.
3. Under **Branch**, select `main` and `/ (root)`, then save.
4. Your app will be live at `https://<username>.github.io/<repo>/`.

## Tech

Single HTML file with plain HTML, CSS and JavaScript. External resources are the Roboto Flex and Noto Naskh Arabic fonts from Google Fonts (with system fallbacks) and, only if you add a key, the Gemini API.

## Privacy

Everything stays in your browser. Counts and photos are never uploaded anywhere. If you turn on the AI reader, the screenshots you upload are sent to Google's Gemini API using your own key.

## License

MIT
