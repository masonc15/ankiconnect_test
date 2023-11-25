# AnkiGPT Assistant

Creating a custom ChatGPT that can interface with my personal Anki collection via the AnkiConnect API.

## Requirements

- **AnkiConnect add-on**: Installed in Anki ([Get the Add-on](https://ankiweb.net/shared/info/2055492159))
- **API endpoint**: AnkiConnect default endpoint `localhost:8765` exposed publicly. (I used ngrok)
- **AnkiConnect settings**: `webCorsOriginList` set to `"*"` in the Anki add-on configuration

## Configuration Steps

- Edit `openapi.json`, replacing the `url` value with your ngrok URL.
- Create a [custom GPT](https://chat.openai.com/gpts/editor) , adding a custom action with the schema from `openapi.json` pasted in.

## Final Notes

- Your custom GPT should now be able to interact with your Anki collection.
