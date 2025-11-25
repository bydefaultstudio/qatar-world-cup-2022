# Qatar Airways 300x600 Display Ad

A Google Web Designer (GWD) banner advertisement for Qatar Airways, designed for 300x600 pixel display placements.

## Overview

This is an interactive video-based display ad that promotes Qatar Airways' sponsorship of the FIFA World Cup 2026. The ad features an autoplaying video background with overlay graphics and a click-through call-to-action.

## Functionality

### Core Features

- **Video Background**: Autoplaying, looping video (`vdo_300x600.mp4`) that serves as the primary visual element
- **Video Poster**: Static image (`vdo_300x600.jpg`) displayed before video loads
- **Click-Through Area**: Entire ad surface (300x600px) is clickable and redirects to the Qatar Airways sponsorship page
- **Exit Tracking**: Integrated with Google's Enabler API for exit link tracking and metrics

### Visual Components

1. **Header Logo**: Qatar Airways logo (`qarar-header.png`) positioned at the top center
2. **Video Background**: Full-screen video covering the entire ad area
3. **Gradient Overlay**: Dark gradient at the bottom for text readability
4. **Copy Text**: SVG text element (`copy.svg`) with promotional messaging
5. **Button**: Styled button with text (`btn-text.svg`) positioned at the bottom

### Technical Implementation

- **Framework**: Google Web Designer 16.4.0 (Banner 3.0.0 template)
- **Ad Format**: Standard 300x600 banner
- **Polite Load**: Enabled for better performance (loads after page content)
- **Video Tracking**: Integrated video metrics tracking via Google's video reporter
- **Exit URL**: `https://www.qatarairways.com/en/sponsorship/fifa-world-cup-26.html`

### User Interaction

- **Click/Tap**: Clicking anywhere on the ad triggers an exit to the Qatar Airways sponsorship page
- **Video Playback**: Video autoplays, loops, and is muted (standard for display ads)
- **Responsive**: Maintains 300x600 aspect ratio across devices

## File Structure

```
├── index.html              # Main ad HTML file
├── vdo_300x600.mp4         # Video background
├── vdo_300x600.jpg         # Video poster/fallback image
├── qarar-header.png        # Qatar Airways header logo
├── copy.svg                # Promotional copy text
├── btn-text.svg            # Button text element
└── backup.jpg              # Backup image asset
```

## Deployment

This ad is designed to be served through Google's ad serving platforms (Google Ads, Display & Video 360) using the Enabler.js API. The ad includes:

- GCD (Google Creative ID) meta tag for tracking
- Enabler.js integration for ad lifecycle management
- Video reporting and exit tracking
- Metric configuration for analytics

## Browser Compatibility

Compatible with modern browsers that support:
- HTML5 video
- Custom Elements (Web Components)
- CSS3 transitions and transforms

## Notes

- Video is set to autoplay, loop, and muted (required for most ad networks)
- The ad uses polite loading to improve page performance
- All exit tracking is handled through Google's Enabler API
- The ad is optimized for 300x600 pixel placements

