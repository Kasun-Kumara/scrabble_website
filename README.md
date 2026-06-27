# Scrablify

Scrablify is a premium React/Tailwind showcase website for a first-year robotics hardware project where a human plays Scrabble against a robot.

## Development

Install dependencies:

```bash
npm install
```

Start the local development server:

```bash
npm run dev
```

## Connect to the Python game

1. Connect the website computer and Python-app computer to the same hotspot.
2. Run `python .\main.py` on the Python-app computer and allow Python through the Windows firewall for private networks if prompted.
3. In the Python app's **Game State** panel, copy the `Website feed` address (for example, `http://192.168.1.20:8765`).
4. Open the Scrablify website, paste that address into the live-match connection field, and select **Connect**.

The website remembers the address and reads the two scores, current player, two-minute turn countdown, cart countdown, and latest 12x12 board grid from the Python app. The computers do not need internet access after the site dependencies are installed.

For a fixed setup, copy `.env.example` to `.env` and set the Python computer's hotspot IP address before starting or building the website.

Build for production:

```bash
npm run build
```

## Current Sections

- `/` home and project introduction
- `/overview` project overview, technical positioning, and dashboard preview
- `/system` system architecture and turn workflow
- `/hardware` hardware module placeholders
- `/team` team members, structure, skills matrix, advisor, and achievements
