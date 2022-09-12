```bash
curl -H "Host: www.producthunt.com" 
     -H "Cookie: _producthunt_session_production=TOKEN" 
     -H "content-type: application/json" 
     -H "tracestate: 1864113@nr=0-1-1864113-594337822-84bde7ea4de690be----1663015167111" 
     -H "accept: */*" 
     -H "newrelic: eyJ2IjpbMCwxXSwiZCI6eyJ0eSI6IkJyb3dzZXIiLCJhYyI6IjE4NjQxMTMiLCJhcCI6IjU5NDMzNzgyMiIsImlkIjoiODRiZGU3ZWE0ZGU2OTBiZSIsInRyIjoiNjk2MjczMTEwYzcxZDFmNDE0ZjcxOTY3OTAzNDU0YTEiLCJ0aSI6MTY2MzAxNTE2NzExMX19" 
     -H "x-requested-with: XMLHttpRequest" 
     -H "accept-language: en-US,en;q=0.9" 
     -H "origin: https://www.producthunt.com" 
     -H "user-agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/15.6.1 Safari/605.1.15" 
     -H "referer: https://www.producthunt.com/my/upcoming/new" 
     -H "traceparent: 00-696273110c71d1f414f71967903454a1-84bde7ea4de690be-01" -
     -data-binary "{\"operationName\":\"UpcomingPageCreate\",\"variables\":{\"input\":{\"name\":\"Landing.Page.as\",\"tagline\":\"Instant Landing Pages hosted on GitHub Pages\",\"thumbnailUuid\":null,\"logoUuid\":null,\"whoText\":\"<p>Hi, I&#x27;m Nathan Clevenger</p>\",\"whatText\":\"<p>We are working on a new exciting product...</p>\",\"media\":null,\"whyText\":\"<p>Get early access before we launch on Product Hunt...</p>\",\"successText\":\"<p>Thank you for supporting our project!</p><p></p>\",\"templateName\":\"default\",\"brandColor\":\"#f64900\",\"backgroundColor\":\"#000\",\"backgroundImageUuid\":null,\"websiteUrl\":\"https://landing.pages.as\",\"appStoreUrl\":null,\"playStoreUrl\":null,\"facebookUrl\":null,\"twitterUrl\":null,\"angellistUrl\":null,\"privacyPolicyUrl\":null,\"hiring\":false,\"status\":\"unlisted\"}},\"query\":\"mutation UpcomingPageCreate($input:UpcomingPageCreateInput!){response:upcomingPageCreate(input:$input){node{id slug __typename}errors{field messages __typename}__typename}}\"}" --compressed "https://www.producthunt.com/frontend/graphql"
```

```json
{
	"operationName": "UpcomingPageCreate",
	"variables": {
		"input": {
			"name": "Landing.Page.as",
			"tagline": "Instant Landing Pages hosted on GitHub Pages",
			"thumbnailUuid": null,
			"logoUuid": null,
			"whoText": "<p>Hi, I&#x27;m Nathan Clevenger</p>",
			"whatText": "<p>We are working on a new exciting product...</p>",
			"media": null,
			"whyText": "<p>Get early access before we launch on Product Hunt...</p>",
			"successText": "<p>Thank you for supporting our project!</p><p></p>",
			"templateName": "default",
			"brandColor": "#f64900",
			"backgroundColor": "#000",
			"backgroundImageUuid": null,
			"websiteUrl": "https://landing.pages.as",
			"appStoreUrl": null,
			"playStoreUrl": null,
			"facebookUrl": null,
			"twitterUrl": null,
			"angellistUrl": null,
			"privacyPolicyUrl": null,
			"hiring": false,
			"status": "unlisted"
		}
	},
	"query": "mutation UpcomingPageCreate($input:UpcomingPageCreateInput!){response:upcomingPageCreate(input:$input){node{id slug __typename}errors{field messages __typename}__typename}}"
}
```
