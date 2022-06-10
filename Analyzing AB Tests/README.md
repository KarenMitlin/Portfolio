<h1 align="center">
Analyzing A/B Tests
</h1>
<p align="center">
 <a href="https://nbviewer.org/github/KarenMitlin/Portfolio-Practicum-Projects/blob/main/Analyzing%20AB%20Tests/AB%20Testing.ipynb">Project</a><br>
</p>
In this project we analyzed two A/B tests that weren't done properly and came to conclusions regarding the way they were performed.
<h2>Project Description</h2>
<h3>Technical Description:</h3>

- <b>Test name:</b> recommender_system_test
- <b>Groups:</b> А (control), B (new payment funnel)
- <b>Launch date:</b> 2020-12-07
- <b>Date when they stopped taking up new users:</b> 2020-12-21
- <b>End date:</b> 2021-01-01
- <b>Audience:</b> 15% of the new users from the EU region
- <b>Purpose of the test:</b> testing changes related to the introduction of an improved recommendation system
- <b>Expected result:</b> within 14 days of signing up, users will show better conversion into product page views (the product_page event), instances of adding items to the shopping cart (product_cart), and purchases (purchase). At each stage of the funnel product_page → product_cart → purchase, there will be at least a 10% increase.
- <b>Expected number of test participants:</b> 6000
<h3>Description of the data:</h3>

<b>'ab_project_marketing_events_us.csv' — the calendar of marketing events for 2020</b>
- <b>name:</b> the name of the marketing event
- <b>regions:</b> regions where the ad campaign will be held
- <b>start_dt:</b> campaign start date
- <b>finish_dt:</b> campaign end date


<b>'final_ab_new_users_upd_us.csv' — all users who signed up in the online store from December 7 to 21, 2020</b>
- <b>user_id</b>
- <b>first_date:</b> sign-up date
- <b>region</b>
- <b>device:</b> device used to sign up


<b>'final_ab_events_upd_us.csv' — all events of the new users within the period from December 7, 2020 through January 1, 2021</b>
- <b>user_id</b>
- <b>event_dt:</b> event date and time
- <b>event_name:</b> event type name
- <b>details:</b> additional data on the event (for instance, the order total in USD for purchase events)


<b>'final_ab_participants_upd_us.csv' — table containing test participants</b>
- <b>user_id</b>
- <b>ab_test:</b> test name
- <b>group:</b> the test group the user belonged to
