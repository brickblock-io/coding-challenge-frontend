# Brickblock Coding Challenge - Frontend

## The Task
Your task is to build a small React app that visualizes our ICO contributions from Pre and Main ICO in a meaningful way.

## What you'll need

1. The [Brickblock Styleguide](./brickblock-styleguide.sketch) that is in this repo. You'll find colors, typography, grids, spacing and certain elements in it. You don't have to follow it to the last pixel but the app should have a Brickblock look & feel.
1. The fonts in the [fonts directory](./fonts)
2. The API endpoint where you'll take the data from is [https://blockchain.brickblock.io/inputs](https://blockchain.brickblock.io/inputs) — this will return the following exemplary data structure:

    ```js
    {
        "preIco": [
            {
                "address": "710a5f86f59c4215db3f6a9c8f0213bc5389d939", // An Ethereum, Bitcoin or Litecoin address that contributed to our Pre ICO in August 2017
                "currency": "ETH", // Can be "ETH", "BTC" or "LTC"
                "value": 100000000000000000, // The contributed amount in the smallest possible unit (e.g. "wei" for Ethereum contributions, or "satoshi" for Bitcoin contributions
                "txid": "d137a652c618a1632f7a1961eb39da48abccd787cf7c49b82039e0fc37145b8c" // The transaction ID of this contribution
            },
            ...
        ],
        "ico": [
            {
                "address": "183nLVZFt3W6G79o5Yx8bTiEBsjER9eMVZ", // An Ethereum, Bitcoin or Litecoin address that contributed to our Main ICO in Novemver 2017
                "currency": "BTC", // Can be "ETH", "BTC" or "LTC"
                "value": 504114, // The contributed amount in the smallest possible unit (e.g. "wei" for Ethereum contributions, or "satoshi" for Bitcoin contributions
                "txid": "f6b48e20e78ed5800ca07ea2a782a14227fee043de86f88eaaebcd88d34c9650" // The transaction ID of this contribution
            },
            ...
        ]
    }
    ```

## The Process

1. Create a new repo wherever you like. Can be GitHub/GitLab/Bitbucket, doesn't matter.
1. In your new repo, create a React app
1. In your app, fetch data from this endpoint: [https://blockchain.brickblock.io/inputs](https://blockchain.brickblock.io/inputs)
1. Visualize this data in a meaningful way. We purposefully leave this very open to see what you can come up with. There's not 1 right solution, but a few example features could be:
    1. Use charts to visualize the data
    2. Filter contributions by currency type
    3. Filter contributions by amount
    4. Filter by Pre and Main ICO
1. Create a README.md explaining how to test the features you have built. Feel free to add additional thoughts, e.g. why you chose certain libraries or why you implemented a feature in a certain way etc.
1. Send us an email to dev@brickblock.io when you're ready to have it reviewed

## Acceptance Criteria
* Your app fetches data from our API and displays it in the UI
* Your app uses redux to manage its state
* Your app is easy to install and run locally

## Bonus Round (not required but nice-to-have)
* Deploy the app somewhere
* Add unit tests
* Add end-to-end tests
* Add flow for static typechecking
* Dockerize the app
* Surprise us…

## Rules
There are not many rules, really. It's all about the result. However, here are a few clarifications:

* Feel free to use as many 3rd party libraries as you'd like.
* It’s ok and even encouraged to look for inspiration elsewhere but if you're taking the lazy way of just copy-and-pasting CodePen snippets: We’ll know.

## How we're evaluating the result
Prioritised from most important to least important, here's our evaluation criteria:

1. UX: Is the app working well on both desktop and mobile?
1. UI: Is the app looking great on both desktop and mobile? Did you just use bootstrap or did you go a step further to make the UI more unique?
1. Code Quality: Is the code clean, well-structured and easy to understand?
1. Performance: Is the app running smoothly? Is there any jank? How does it work with a slow internet connection?
1. The extra mile: Did you write tests? Are code quality tools such as eslint, flow or prettier in place? Is there documentation on how to get the app running?

You do not need to hit all points, but obviously, the more the better :)
