# How They Test

[![Contributions Welcome!](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)

> A curated collection of practical testing techniques, strategies, and best practices. Find step-by-step testing recipes for functional, performance, security, and automation testing. Ideal for testers and developers looking to enhance software quality with actionable insights. 🚀

## Foreword

One of the outcomes of the various [ISQA](TBA) meetups was that many software companies got to share their testing and quality culture with the community. It was absolutely fantastic to see the amazing stuff companies are doing to test their software, and ensure quality of their products and platforms.

Apart from this, many companies regularly come forward and share their best practices, tools, techniques and culture of software testing on various public platforms like conferences, blogs & meetups. The resources are there but dispersed, lost into the internet.

There is no single knowledge repository that gives a direct look at these best practices, tools, techniques and culture of software testing these companies adopt. This repository intends to do that.

Happy Learning!

*Please note, that all the resources mentioned here are publicly available resources.*

## Kind of topics here

Testing / quality of software goes beyond traditional activities of pre-release functional testing and test automation. Hence the kind of topics you can expect to read about here are:

- Functional testing
- Non-functional testing
- Test automation
- Testing in CI/CD
- Release management and it's impact on quality/testing.
- Quality processes and culture
- Testing in production (monitoring/observability, chaos engineering, site reliability engineering etc.)
- Customer / user support
- User research / user testing from product/UX perspective

## Companies & how they test their software

<details>
<summary><b>Allofresh</b> - Food Delivery Platform</summary>

#### Overview
Allofresh is a food delivery platform that connects users with various food vendors. Our testing strategy focuses on ensuring reliable API services, smooth mobile app experience, and comprehensive manual testing.

#### Testing Stack
- **API Testing**: Ruby + RSpec
- **Mobile Testing**: Flutter + Patrol
- **Manual Testing**: Jira/TestRail
- **E2E Testing**: Cypress

#### Testing Approach

##### API Automation
- Ruby-based API testing framework
- RSpec for BDD-style test writing
- HTTParty/RestClient for API requests
- Comprehensive test coverage for all endpoints
- Example:
```ruby
RSpec.describe 'Recipes API' do
  it 'returns list of recipes' do
    response = HTTParty.get('http://api.allofresh.com/v1/recipes')
    expect(response.code).to eq(200)
    expect(JSON.parse(response.body)).to include('recipes')
  end
end
```

##### Mobile App Testing
- Flutter-based mobile testing
- Patrol framework for native device interactions
- Cross-platform testing (iOS & Android)
- Offline functionality testing
- Example:
```dart
patrolTest('Recipe flow test', ($) async {
  await $.pumpWidget(MyApp());
  await $(TextField).enterText('Pasta');
  await $(IconButton).tap();
  expect($(Text).containing('Pasta Recipes'), findsOneWidget);
});
```

##### Manual Testing
- Structured test case management in Jira/TestRail
- Regular smoke testing after deployments
- Comprehensive regression testing before releases
- Exploratory testing for edge cases
- User acceptance testing with stakeholders

#### Quality Processes
- Daily test execution in CI/CD pipeline
- Weekly test case reviews
- Monthly test strategy updates
- Quarterly quality metrics review

#### Tools & Infrastructure
- Test Environment: dev, staging, production
- CI/CD: GitHub Actions
- Test Management: Jira/TestRail
- Monitoring: New Relic, Sentry

#### Best Practices
1. **API Testing**
   - Meaningful test descriptions
   - Success and failure scenarios
   - External dependency mocking
   - Test data cleanup

2. **Mobile Testing**
   - Multiple device testing
   - Offline functionality
   - Deep linking
   - Push notification testing

3. **Manual Testing**
   - Documented test cases
   - Clear bug reports
   - Visual evidence (screenshots/videos)
   - Regular test case updates

#### Resources
- [API Testing Guide](docs/allofresh/api-testing.md)
- [Mobile Testing Guide](docs/allofresh/mobile-testing.md)
- [Manual Testing Guide](docs/allofresh/manual-testing.md)
</details>

## Contributors

<a href="https://github.com/gabesx/testing-recipes-catalogue/graphs/contributors">
  <img src="https://contributors-img.web.app/image?repo=gabesx/testing-recipes-catalogue" />
</a>

## Contribution

Want to contribute? Just fork and raise a PR!

## Credits

- Idea inspired from the [awesome](https://github.com/sindresorhus/awesome) lists.
- Static site powered by [docsify](https://docsify.js.org/).
- Contributors list generated using [contributors-img](https://contrib.rocks/preview?repo=gabesx%2Ftesting-recipes-catalogue)
- All the authors and the companies they represented in the resources.
