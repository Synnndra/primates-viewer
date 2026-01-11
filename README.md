# MidEvil NFT Viewer

A web application to view, sort, filter, and create collages from MidEvil NFTs on the Solana blockchain.

**Live Demo:** https://solana-nft-viewer-lilac.vercel.app

## Features

### NFT Viewing
- **Multi-wallet support** - View NFTs from up to 5 wallets simultaneously
- **MidEvil collection filter** - Automatically filters for MidEvil NFTs, excludes Graveyard
- **NFT details modal** - Click any NFT to view full traits and mint address

### Sorting & Filtering
- **Sort by** - NFT number, background color, or any trait
- **Filter by traits** - Filter NFTs by any trait type
- **Collapsible controls** - Clean UI with expandable sort/filter sections

### Collage Creator
- **Multiple layout options:**
  - Auto-Square - Roughly square grid
  - Wide - More columns than rows (landscape)
  - Tall - More rows than columns (portrait)
  - Twitter Header (3:1) - Optimized for Twitter banners
  - Phone Wallpaper (9:19.5) - Optimized for mobile wallpapers
  - Montage - Mixed sizes with 2x2 featured NFTs

- **Customization:**
  - Adjustable spacing slider (0-30px)
  - Drag-and-drop reordering
  - Size swapping in montage mode
  - Placeholder images for empty spaces

- **Export** - Download collage as high-quality PNG

## How to Use

### Online (Recommended)
Visit https://solana-nft-viewer-lilac.vercel.app

### Local Development

1. **Get a FREE Helius API key:**
   - Go to https://helius.dev
   - Sign up and create an API key
   - Add your key to `api/helius.js`

2. **Run locally:**
   ```bash
   node server.js
   ```
   Then open http://localhost:3000

3. **Or deploy to Vercel:**
   ```bash
   vercel --prod
   ```

## Project Structure

```
solana-nft-viewer/
├── index.html          # Main HTML page
├── style.css           # Medieval-themed styling
├── app.js              # Core application logic
├── server.js           # Local development server
├── api/
│   └── helius.js       # Vercel serverless API proxy
├── vercel.json         # Vercel deployment config
├── Placeholder.jpg     # Placeholder image for collages
└── README.md           # This file
```

## Technologies

- **Frontend:** HTML, CSS, JavaScript (Vanilla)
- **API:** Helius (for compressed NFT support)
- **Deployment:** Vercel
- **Fonts:** Cinzel, MedievalSharp (Google Fonts)

## Example Wallets

Try these wallet addresses:
- `7xKXtg2CW87d97TXJSDpbD5jBkheTqA83TZRuJosgAsU`
- `GUfCR9mK6azb9vcpsxgXyj7XRPAKJd4KMHTTVvtncGgp`

## Collage Layout Guide

| Layout | Best For |
|--------|----------|
| Auto-Square | General purpose, balanced look |
| Wide | Desktop wallpapers, banners |
| Tall | Mobile wallpapers, vertical displays |
| Twitter Header | Social media banners (1500x500) |
| Phone Wallpaper | Mobile lock/home screens |
| Montage | Featured NFTs with mixed sizes |

## License

MIT
