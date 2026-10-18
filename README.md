# Mendi IP Finder

A simple, responsive website that looks up a domain's IPv4 address and attempts to show its approximate IP-based location on an interactive map.

## Features

- Find a domain's IPv4 address using Google Public DNS.
- Display approximate IP geolocation details when the location service is available:
  - City
  - Region
  - Country
  - ISP / network organization
  - Timezone
  - Latitude and longitude
- Show the coordinates on an embedded OpenStreetMap view.
- Open a larger map in OpenStreetMap.
- Copy the IPv4 address or location summary.
- Responsive dark-themed interface.
- No custom backend is required for the basic static website.

## Services used

- **DNS lookup:** [Google Public DNS](https://dns.google/)
- **IP geolocation:** [ipdata.free](https://ipdata.free/)
- **Map:** [OpenStreetMap](https://www.openstreetmap.org/)

The location endpoint is called from the browser. Its availability, usage limits, and browser/CORS behavior can change, so test the published website. If the location lookup fails, the page should still display the IP address when DNS lookup succeeds.

## How to use

1. Open the website.
2. Enter a domain, such as `google.com`.
3. Press **Find IP & Location**.
4. If the location service responds successfully, review the estimated location details and map.

You can enter a domain with or without `https://`, for example `https://example.com/page`.

## Deploy with GitHub Pages

1. Upload `index.html` and `README.md` to the root of your GitHub repository.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Select the `main` branch and the `/(root)` folder, then save.
5. Wait for GitHub Pages to publish the website. The published URL will appear in the Pages section.

## Limitations and privacy

- IP geolocation is approximate. It may indicate an ISP gateway, proxy, VPN, or network provider location rather than a visitor's actual location.
- An IP address cannot reveal someone's exact home address or GPS position by itself.
- Some domains may not return an IPv4 A record.
- The free location endpoint may have usage limits or may stop responding; no uptime or availability is guaranteed.
- Do not use these results to identify or track a person precisely.

## Credits

- **Developed by:** Tahlil
- **AI assistance:** ChatGPT (OpenAI)
- **Built with:** HTML, CSS, and JavaScript
- **Map data:** © OpenStreetMap contributors
