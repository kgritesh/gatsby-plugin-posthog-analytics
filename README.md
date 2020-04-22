# gatsby-plugin-posthog-analytics

![npm](https://img.shields.io/npm/v/gatsby-plugin-posthog-analytics?style=plastic)

A simple gatsby plugin to add [posthog](https://posthog.com/) analytics to your site. Automatically tracks all the pageviews and clicks.

## Install

`yarn add gatsby-plugin-posthog-analytics`

or

`npm install --save gatsby-plugin-posthog-analytics`

## How to use

```javascript
// In your gatsby-config.js
module.exports = {
  plugins: [
    {
      resolve: `gatsby-plugin-posthog-analytics`,
      options: {
        // Specify the API key for your Posthog Project (required)
        apiKey: "YOUR_POSTHOG_ANALYTICS_API_KEY",
	// Specify the app host if self-hosting (optional, default: https://app.posthog.com)
	appHost: "YOUR_POSTHOG_APP_HOST_URL",
        // Puts tracking script in the head instead of the body (optional, default: true)
        head: true,
	// Enable posthog analytics tracking during development (optional, default: false)
	isEnabledDevMode: true
      },
    },
  ],
}
```
