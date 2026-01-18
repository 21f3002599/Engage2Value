Engage2Value

Engage2Value is a machine learning competition focused on predicting customer purchase value using multi-session behavioral data across digital touchpoints. The dataset contains anonymized information such as browsers, traffic sources, devices, and geographic signals. By modeling these patterns, participants estimate each user’s purchase potential to improve targeting, marketing, and engagement strategies.

Description

The goal of this competition is to predict a customer’s purchaseValue based on their behavior across multiple sessions on a digital commerce platform. The dataset captures anonymized user interactions, including browser types, traffic sources, device details, and geographical indicators. Participants will model these signals to estimate purchase potential and support data-driven marketing decisions.

Evaluation

Submissions are evaluated using the R² score (r2_score) between the predicted values and the true target values.

Submission File

For each id in the test set, you must predict the target variable purchaseValue.

Submission format:

id,purchaseValue
0,0
1,0
2,10990000
4,36500
5,0
...

Dataset Description

This dataset contains detailed session-level data from a large-scale digital commerce platform. Each row represents a unique user session and includes information related to user behavior, acquisition channels, device characteristics, and geographic location.

The target variable is purchaseValue, which represents the total amount spent during a session.

Key Feature Categories
1. User Behavior & Session Metrics

totalHits, pageViews, totals.bounces, new_visits, totals.visits: Indicators of user engagement.

sessionNumber, sessionStart: Session sequence and timing information.

2. Device & Technical Attributes

deviceType, os, browser, screenSize, device.browserSize, device.language: Device and browsing environment details.

browserMajor, device.*: Device model, version, and screen specifications.

gclIdPresent: Indicates the presence of a Google Click ID for ad tracking.

3. Traffic & Marketing Source

userChannel, trafficSource, trafficSource.medium, trafficSource.keyword, trafficSource.campaign: User acquisition information.

trafficSource.adwordsClickInfo.*: Advertising-related attributes such as ad network and slot.

trafficSource.adContent, trafficSource.referralPath, trafficSource.isTrueDirect: Additional attribution details.

4. Geographical Context

geoNetwork.city, locationCountry, geoNetwork.continent, geoNetwork.subContinent, geoNetwork.metro, geoNetwork.region: Geographic indicators.

geoCluster, locationZone: Groupings based on geographic or behavioral patterns.

5. Identifiers

userId, sessionId: Unique identifiers enabling multi-session user analysis.

6. Target Variable

purchaseValue: Total amount spent (in currency units) during the session. This is the variable to be predicted.
