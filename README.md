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
<summary><b>AlloFresh</b> - Online Grocery Shopping Platform</summary>

#### Overview
AlloFresh is an online grocery shopping platform managed by PT Allo Fresh Indonesia. The platform provides daily necessities including food, beverages, personal care products, and household items. AlloFresh is accessible through mobile applications available on Play Store and App Store, offering quick delivery services (as fast as 30 minutes for certain products) across various cities in Indonesia.

#### Company Background
- **Parent Company**: PT Allo Fresh Indonesia
- **Partnership**: Collaboration between Trans Retail Indonesia (CT Corp business unit), Bukalapak, and Growtheum Capital Partners
- **Presence**: Multiple cities in Indonesia including Malang, Surabaya, Makassar, and Palembang

#### Key Features
- Online grocery shopping platform
- Mobile applications (iOS & Android)
- Comprehensive product range
- Quick delivery service (2-hour or 30-minute options)

#### Testing Stack
- **API Testing**: Ruby + RSpec
  - Custom test framework for API validation
  - Integration with CI/CD pipeline
  - Automated test reporting

- **Mobile Testing**: Flutter + Patrol
  - Cross-platform test automation
  - Native device interaction testing
  - Performance monitoring

- **Manual Testing**: Jira/In House TcMS powered by QaraTMS
  - Open-source test management system based on [QaraTMS](https://github.com/a13xh7/QaraTMS)
  - Features:
    - Test repository management
    - Test suite organization
    - Test case versioning
    - Test plan creation and execution
    - Test run tracking
    - Documentation module
    - Project-based organization
    - Role-based access control
  - Integration with Jira for bug tracking
  - Test execution tracking and reporting
  - Test environment management
  - Test data management

#### Testing Approach

##### API Automation
- Ruby-based API testing framework
- RSpec for BDD-style test writing
- HTTParty/RestClient for API requests
- Comprehensive test coverage for all endpoints
- Automated test data setup and cleanup
- Environment-specific test configurations
- Performance testing integration
- Security testing scenarios

##### Mobile App Testing
- Flutter-based mobile testing
- Patrol framework for native device interactions
- Cross-platform testing (iOS & Android)
- Offline functionality testing
- Push notification testing
- Deep linking validation
- App state management testing
- Performance and memory testing
- Device-specific test scenarios

##### Manual Testing
- Structured test case management in QaraTMS
- Test repository organization by project modules
- Test suite and test case management
- Test plan creation and execution
- Test run tracking and reporting
- Bug tracking integration with Jira
- Test environment management
- Test data management
- Test case version control
- Test execution metrics

#### Quality Processes
- **Test Planning**
  - Feature-based test planning
  - Test case design and review
  - Test environment setup
  - Test data preparation

- **Test Execution**
  - Daily smoke testing
  - Feature-specific test execution
  - Regression testing
  - Performance testing
  - Security testing

- **Test Management**
  - Test case version control
  - Test execution tracking
  - Bug tracking and management
  - Test metrics collection
  - Quality reporting

- **Continuous Improvement**
  - Weekly test case reviews
  - Monthly test strategy updates
  - Quarterly quality metrics review
  - Test process optimization

#### Tools & Infrastructure
- Test Environment: dev, staging, production
- CI/CD: GitHub Actions
- Test Management: Jira/In House TcMS powered by QaraTMS
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
