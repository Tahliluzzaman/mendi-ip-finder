# Mendi IP Finder

A lightweight website that looks up a domain's IPv4 address using Google Public DNS. Built with HTML, CSS, and JavaScript—no Python backend required.

**Developer:** Tahlil  
**AI Assistance:** ChatGPT (OpenAI)

## Features

- Look up a domain's IPv4 (A) DNS record
- Copy the returned IP address
- Responsive design for mobile and desktop
- No API key or backend server required

## Run locally

Open `index.html` in a modern browser with an internet connection.

## Publish with GitHub Pages

1. Upload `index.html` and `README.md` to the root of a GitHub repository.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and `/ (root)` folder, then save.
5. Open the URL shown in the Pages settings after deployment finishes.

## Notes and limitations

- DNS lookup requires an internet connection.
- This tool displays one IPv4 address (A record) when one is returned. A domain may have multiple addresses or only IPv6 (AAAA) records.
- DNS responses can differ from the result returned by a local operating system's resolver.
- An IP address does not reliably reveal a website owner's physical location.
- Google Public DNS is an external service, so availability depends on that service and the user's network.

## Credits

Developed by **Tahlil**. AI assistance by **ChatGPT (OpenAI)**. DNS lookup requests use the Google Public DNS-over-HTTPS JSON API.
