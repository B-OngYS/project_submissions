Project 2: HDB resale prices


# Introduction

Housing agents have many avenues to advertise to resale flat buyers. In the past, agents will often publish advertisments on newspapers so they have to be careful with what features they use to advertise and what price they should put up as the newspapers charge per letter.

Now, the problem is too much information, what do agents put up in PropertyGuru or 99.co for maximum impact for their advertisments?

We will generate several models to help these agents decide.

### Problem Statement

ResaleLeiLong is a HDB resale social network that offers a price estimator and feature recommendation service for housing agents.

Agents need to know what is a reasonable price to recommend to buyers and sellers and they also need to know what features will affect to price when communicating with their clients.

---

### Datasets
The data set is taken from the Kaggle competition on HDB prices (https://www.kaggle.com/competitions/dsi-sg-project-2-regression-challenge-hdb-price/overview).

The data dictionary can be found on that website as well.

### Key takeaways

- Many features like schools and MRTs correlate pretty strongly with their planning area, making it difficult to account for their effects.
- For each planning area can be considered afforable or expensive based on the type of flat. For example, relative to other flat types in other areas, Ang Mo Kio is an afforable area for 4 room flats but expensive for 5 room flats.
- The effect of the number of hawker centres within a 2km radius was only significant for 4 room, 5 room, and executive flats.
- Only the 1 room flats were affected by transaction year, meaning that over time, the other flats had more or less the same value. This might be due to government measures cooling the resale market.
- Flat type and model is a better predictor of resale price than floor area.
- Our lasso, ridge, and linear regression models turned out to be pretty similar, there might not be enough unique features to help expain resale prices.

### Recommendations

- We will need more data like the state of the flat (move in condition, renovated), closeness to the expressway or other metrics.
- As a production model, we can tell housing agents that within a 66k range, they can use our price estimator.
- Agents should not waste space publishing too many details on their adverts.
