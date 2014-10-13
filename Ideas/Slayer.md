1. Birth of the idea

In digital products big chunk of users churn every month.
User lifetime and retention is 20-40% and needs to be optimized. Also user engagement can be better in most cases.
Wanted to build a social layer for the football vertical to create defensibility and increase user retention. Other example for successful approach is Spotify.
Tried multiple things, one-to-many didn't work - users want 1 to 1 communication or 1-to-n with friends (mail shares in data).
MVP is not messages but users and connections.

Hypothesis:
A social layer can impact retention and engagement in almost any digital product (except a few verticals finance, medicine etc.).

2. Defining the problem

User perspective

Users act in silos when they're using digital products even though probably they have friends using some of the same products. An example is a user who uses a news app. If the app would tell him that of his friends read article XYZ, there is a chance he clicks that too, discovers interesting content and likes the product more.

There are similar assumptions for gaming products. Leaderboards among friends or event based notification such as: "Your friend finished level 20" etc. will have a positive impact of the users experience with the product. He not only comes back to play but also to check what their friends have done.

We assume this approach works for almost any vertical.

Product perspective

Digital products especially startups suffer with monthly churned users, low retention rates and sometimes low engagement. Some spend money to acquire users and it turns out that most of them where "empty calories".

As technologies evolve it is extremely easy for competitors to create similar products and more easy for the user to switch as there are no switchover costs what so ever.

This means digital products need to be unique in terms of the user experience and have something that others don't. A social layer to create user connections and build some of a communication layer on top is a potential solution. The integration should be as seamless as possible --> a plug and play SDK open-sourced on github.

3. Selling the idea

You wouldn't build google maps if you were to develop a map app. You probably also wouldn't reinvent payment systems but rather use paypal or stripe, as they have proven a robust and scalable system in that vertical.

The reason for that is, you shouldn't loose focus and concentrate on your core product you build for the users.

The same goes for a social layer. A social layer is not just a user database. It means creating users, storing relevant information about them, creating connections and collecting events depending on their usage. That is a highly complex field with lots of bigdata and all it's challenges. We can build a real-world generic social layer thats serves all that.

Core pillars

1. Users
2. Connections
3. Events/Notifications

User connections are essential. One benefit of the mobile ecosystem is that most the users have the phone number of their friends. A few have E-Mail addresses and the rest of our connections live in social networks, namely: facebook, twitter, linkedin etc.

By creating an intelligent API to store all relevant user information with necessarily a registration flow in the product is the first step in the process.
The second step is to create connections based on either the phone number and address book or e-mail or social media graphs.
The third step is to collect behaviour based events of the users and intelligently map those their connections. The MVP of that is a simple activity feed to communicate friends activity in the app.

4. Rise of the vision

The social layer is a service which has the potential to be the biggest generic social layer across  multiple products. Despite the fact the all the customer data is protected and encrypted the potential reach is huge.

Thus monetization models such as sponsored placements in the activity feed highly target based of user attributes and behavior are potential revenue streams with a free tier for customers. Another model are SaaS based pricing tiers based on number of users or events.

5. Coming back to business

As this is a highly complex and technical approach the MVP needs to have a backend which can handle user information. Potentially it should be able to GET user friends lists (phonebook or facebook) and create connections. On the cient-side an iOS and later Android SDK is needed. They need to be lightweight and performant to not create implementation blockers.

For the backend 2-3 experienced backend engineers are needed. Of them should specialize on large-scale data and machine learning, the others on infrastructure and API. For the SDK's one dedicated iOS developer and one Android is needed.

Berlin is a very suitable location as there the costs for qualified engineering resource is comparably low and it's an attractive city to recruit from all over the world. Also investors are more and more tempted to invest in the berlin ecosystem.

Competition
http://getsocialize.com/
http://www.sharethis.com/
https://github.com/socialize/socialize-sdk-ios
https://stormpath.com/
