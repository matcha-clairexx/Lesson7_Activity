# Lesson7_Activity
## Slide 16 quick-check answers


**Q1. Why should most tests be feature tests?**

Feature tests exercise the application through real routes, middleware, controllers, and the database, so they verify that the pieces work together.


**Q2. What would go wrong without `RefreshDatabase`?**

Test data could persist or leak between tests, making results depend on test order or old database records. Each test should start with a clean database state.


**Q3. Why test the stranger case, not just the owner?**

The owner test proves access is allowed; the stranger test proves unauthorized users are denied and cannot change someone else’s data. It catches missing or broken policy checks.
