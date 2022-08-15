# Software Requirements

## Vision

An application that gathers and displays the stock trading activity of members of Congress.  Senators and representatives are potentially privy to information relevant to the price of stocks, and public knowledge of the stock trading activity of Congress members might shed light on, or at least deter, insider trading.

*Disclaimer*: this app exists purely for informational purposes.  Neither this app nor its authors make any inference to the intent behind any Congress member's stock trading activity. Further, nothing provided by this app should be interpreted as financial advice, as it is not.  

## Scope

- In
  - The web app will display the previous year performance of the S&P 500 on a graph
  - Users will be able to choose the portfolios of Congress members to compare against the S&P 500
  - Users will be able to find out who their representatives are
  - Users will be able to create an account and logging
    - So that they can save their representatives to their account to follow their activity
    - So that they can subscribe to email alerts

- Out
  - This app will not become an API

- Minimum Viable product
  - Graph showing S&P 500 and selected members of Congress portfolio performance
  - List of 50 most recent trades by all of Congress

- Stretch
  - Email subscription (weekly digest of recent trades)

## Functional Requirements

- User can see previous year's performance of S&P 500
- User can see performance of selected Congress members' portfolios
- User can create an account and log in to it
- User can find which representatives serve a given locale
- Users can save representatives to their account to track
- Users can subscribe to email alerts

## Non-Functional Requirements

### Security

- Users will have the option to sign up for an account which will be done with basic and bearer auth

### Testability

Using Jest and Supertest, CRUD routes will be tested for returning expected data and status code, as well as expected status codes for errors. Also basic and bearer auth should properly execute and allow for/not allow user actions depending on their role.
