# Engage2Value

Engage2Value is a machine learning competition focused on predicting customer purchase value using multi-session behavioral data across digital touchpoints. The dataset contains anonymized information such as browsers, traffic sources, devices, and geographic signals. By modeling these patterns, participants estimate each user’s purchase potential to improve targeting, marketing, and engagement strategies.


🔗 **Kaggle Competition:**  
[https://www.kaggle.com/competitions/your-competition-name](https://www.kaggle.com/competitions/engage-2-value-from-clicks-to-conversions/overview)

# Description

The goal of this competition is to predict a customer’s purchaseValue based on their behavior across multiple sessions on a digital commerce platform. The dataset captures anonymized user interactions, including browser types, traffic sources, device details, and geographical indicators. Participants will model these signals to estimate purchase potential and support data-driven marketing decisions.

# Evaluation

Submissions are evaluated using the R² score (r2_score) between the predicted values and the true target values.

Submission File

For each id in the test set, you must predict the target variable purchaseValue.

Submission Format
| id | purchaseValue |
| -- | ------------- |
| 0  | 0             |
| 1  | 0             |
| 2  | 10990000      |
| 4  | 36500         |
| 5  | 0             |
| …  | …             |


This dataset contains detailed session-level data from a large-scale digital commerce platform. Each row represents a unique user session and includes information related to user behavior, acquisition channels, device characteristics, and geographic location.

The target variable is purchaseValue, which represents the total amount spent during a session.

# Key Feature Categories

    User Behavior & Session Metrics
        totalHits, pageViews, totals.bounces, new_visits, totals.visits: Indicators of user engagement and session activity.
        sessionNumber, sessionStart: Information related to session sequence and timing.

    Device & Technical Attributes
        deviceType, os, browser, screenSize, device.browserSize, device.language: Details about the user's device and browsing environment.
        browserMajor, device.*: Encompasses a variety of device-level descriptors such as model, version, and screen specifications.
        gclIdPresent: Signals the presence of a Google Click ID used in ad tracking.

    Traffic & Marketing Source
        userChannel, trafficSource, trafficSource.medium, trafficSource.keyword, trafficSource.campaign: Insights into how users arrived at the platform.
        trafficSource.adwordsClickInfo.*: Contains attributes from advertising sources, including ad network type and slot.
        trafficSource.adContent, trafficSource.referralPath, trafficSource.isTrueDirect: Provide further attribution details.

    Geographical Context
        geoNetwork.city, locationCountry, geoNetwork.continent, geoNetwork.subContinent, geoNetwork.metro, geoNetwork.region: Geographic identifiers to help understand regional behavior trends.
        geoCluster, locationZone: Groupings based on geographic or behavioral patterns.

    Identifiers
        userId, sessionId: Unique identifiers for each user and session, allowing for multi-session analysis.

    Target Variable
        purchaseValue: The amount (in currency units) spent by the customer during the session. This is the target variable to be predicted.
