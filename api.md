```bash
curl -H "Host: www.producthunt.com" 
     -H "Cookie: _producthunt_session_production=TOKEN" 
     -H "content-type: application/json" 
     -H "accept: */*" 
     -H "x-requested-with: XMLHttpRequest" 
     -H "accept-language: en-US,en;q=0.9" 
     -H "origin: https://www.producthunt.com" 
     -H "user-agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/15.6.1 Safari/605.1.15" 
     -H "referer: https://www.producthunt.com/my/upcoming/new" 
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

```json
{
	"operationName": "SaveUpcomingPage",
	"variables": {
		"input": {
			"whoText": "<p>Hi, I&#x27;m Nathan Clevenger</p>",
			"whatText": "<p>We are working on a new exciting product...</p>",
			"media": null,
			"whyText": "<p>Get early access before we launch on Product Hunt...</p>",
			"successText": "<p>Thank you for supporting our project!</p><p></p>",
			"upcomingPageId": "196139"
		},
		"reloadVariant": false
	},
	"query": "mutation SaveUpcomingPage($input:UpdateUpcomingPageInput!$reloadVariant:Boolean!){response:updateUpcomingPage(input:$input){node{id ...UpcomingPageLayoutControlsForm variant(preferredKind:\"b\")@include(if:$reloadVariant){id __typename}__typename}errors{field messages __typename}__typename}}fragment UpcomingPageLayoutControlsForm on UpcomingPage{id accountId angellistUrl appStoreUrl availableTemplateNames canManageShipAb canPromoteUpcomingPage facebookUrl hiring name playStoreUrl privacyPolicyUrl seoDescription seoImageUuid seoTitle slug status subscriberCount successText tagline thumbnailUuid topicIds twitterUrl updatedAt webhookUrl websiteUrl widgetIntroMessage variants{id backgroundColor backgroundImageUuid brandColor kind logoUuid templateName thumbnailUuid unsplashBackgroundUrl whatText whoText whyText media{...Media __typename}__typename}...MetaTags __typename}fragment Media on Media{imageUuid mediaType originalWidth originalHeight metadata{url platform videoId __typename}__typename}fragment MetaTags on SEOInterface{id meta{canonicalUrl creator description image mobileAppUrl oembedUrl robots title type author authorUrl __typename}__typename}"
}
```
```json
{
	"operationName": "SaveUpcomingPage",
	"variables": {
		"input": {
			"seoTitle": "Title",
			"seoDescription": "Description",
			"seoImageUuid": null,
			"upcomingPageId": "196139"
		},
		"reloadVariant": false
	},
	"query": "mutation SaveUpcomingPage($input:UpdateUpcomingPageInput!$reloadVariant:Boolean!){response:updateUpcomingPage(input:$input){node{id ...UpcomingPageLayoutControlsForm variant(preferredKind:\"b\")@include(if:$reloadVariant){id __typename}__typename}errors{field messages __typename}__typename}}fragment UpcomingPageLayoutControlsForm on UpcomingPage{id accountId angellistUrl appStoreUrl availableTemplateNames canManageShipAb canPromoteUpcomingPage facebookUrl hiring name playStoreUrl privacyPolicyUrl seoDescription seoImageUuid seoTitle slug status subscriberCount successText tagline thumbnailUuid topicIds twitterUrl updatedAt webhookUrl websiteUrl widgetIntroMessage variants{id backgroundColor backgroundImageUuid brandColor kind logoUuid templateName thumbnailUuid unsplashBackgroundUrl whatText whoText whyText media{...Media __typename}__typename}...MetaTags __typename}fragment Media on Media{imageUuid mediaType originalWidth originalHeight metadata{url platform videoId __typename}__typename}fragment MetaTags on SEOInterface{id meta{canonicalUrl creator description image mobileAppUrl oembedUrl robots title type author authorUrl __typename}__typename}"
}
```
```json
{
	"operationName": "SaveUpcomingPage",
	"variables": {
		"input": {
			"templateName": "cinematic",
			"logoUuid": null,
			"brandColor": "#f64900",
			"backgroundColor": "#000",
			"backgroundImageUuid": null,
			"upcomingPageId": "196139"
		},
		"reloadVariant": false
	},
	"query": "mutation SaveUpcomingPage($input:UpdateUpcomingPageInput!$reloadVariant:Boolean!){response:updateUpcomingPage(input:$input){node{id ...UpcomingPageLayoutControlsForm variant(preferredKind:\"b\")@include(if:$reloadVariant){id __typename}__typename}errors{field messages __typename}__typename}}fragment UpcomingPageLayoutControlsForm on UpcomingPage{id accountId angellistUrl appStoreUrl availableTemplateNames canManageShipAb canPromoteUpcomingPage facebookUrl hiring name playStoreUrl privacyPolicyUrl seoDescription seoImageUuid seoTitle slug status subscriberCount successText tagline thumbnailUuid topicIds twitterUrl updatedAt webhookUrl websiteUrl widgetIntroMessage variants{id backgroundColor backgroundImageUuid brandColor kind logoUuid templateName thumbnailUuid unsplashBackgroundUrl whatText whoText whyText media{...Media __typename}__typename}...MetaTags __typename}fragment Media on Media{imageUuid mediaType originalWidth originalHeight metadata{url platform videoId __typename}__typename}fragment MetaTags on SEOInterface{id meta{canonicalUrl creator description image mobileAppUrl oembedUrl robots title type author authorUrl __typename}__typename}"
}
```
