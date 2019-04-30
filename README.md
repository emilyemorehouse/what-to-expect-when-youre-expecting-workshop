# What To Expect When You're Expecting

This repository holds all materials for the PyCon 2019 workshop presented by Emily Morehouse.

## Summary

We all know we should be testing our applications, but testing is hard and great testing is even
harder.

Take a deep dive into what types of things to test and how to approach testing them in your Django
apps, plus learn how to leverage modern headless browser libraries and automated visual diff-ing to
get (and keep) pixel-perfect apps.

We'll cover types of testing as a whole, plus practical applications and deep dives for testing in
Django and visual regression testing with Javascript (whether for templates rendered by Django or
for a standalone Javascript client application).

## Audience Expectations

A foundational knowledge of Python and a web framework of choice is beneficial, as we'll dive right
into testing an existing application. Starter code and code progressions will be provided, so you
don't have to be a Django expert to grasp the content! Whether you love, hate, or have never used
Javascript, you'll feel at home; our use of JS will be limited to leveraging libraries to gather
data and screenshots for visual regression testing, whether for a JS client or a Django web app.

## 💅🏻 Pre-Workshop Prep

To start, you'll want to clone the repository to your local machine. Though there is an option to
download a zipfile of the contents, it is recommended to clone using Git so you can navigate to
different branches and commits in the code.

If you need to install Git, please see: [Getting Started Installing
Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

Clone the repository:

```sh
git clone git@github.com:emilyemorehouse/what-to-expect-when-youre-expecting-workshop.git
```

Next, you should install dependencies for the two applications we'll be working on. Make sure you
set up both per the instructions below:

### Install dependencies for our React app

If you don't have Node installed, you should install that first: https://nodejs.org/en/download/

This repository is tested with Node v.8.12, so use other versions at your own risk.

```sh
git checkout visual-init
cd agnostic-visual-regression-testing/code
npm install
npm run start
```

### Install dependencies for our Django app

You'll need Python 3.6+ installed. If you don't have that set up, see:
https://www.python.org/downloads/

```sh
git checkout django-init
cd regression-testing-in-django/code
```

See [Step 0](regression-testing-in-django/notes/00_setup.md) for full instructions on installing
dependencies, configuration, and running the app.

---

## 👩🏻‍🏫 How To Use This Repository

There are branches for each type of testing that we will cover:

- "Regression Testing in Django" uses branch `django-walkthrough`
- "Visual Regression Testing with Javascript" uses branch `visual-tests-walkthrough`

Each branch has commits per-step, which means that you'll want to checkout a previous version if
you want to follow along.

Here's a sample workflow for navigating through the repo:

```sh
# Check out to final step on `django-walkthrough` branch
git checkout django-walkthrough

# List commits to go back to a specific step, or get the commit hash (id) from
# https://github.com/emilyemorehouse/what-to-expect-when-youre-expecting-pycon-workshop/commits/django-walkthrough
git log

# Checkout the specific commit you want to work from
git checkout <commit-hash>
```

You can opt to start from the initial step and work through implementing all of the changes on your
own using the committed steps to follow along if you get lost, or you can checkout each step along
the way to ensure that you understand each step. It really depends on your comfort level with the
material and how you learn best!

## 📽 Slides

Online: [Link](https://emilyemorehouse.github.io/what-to-expect-when-youre-expecting/)

## 📝 Content and Notes

1. Introduction
1. Foundational Knowledge for Testing
1. [Walkthrough - Regression Testing in Django](regression-testing-in-django/README.md)
1. [Walkthrough - Visual Regression Testing Powered By
   Javascript](agnostic-visual-regression-testing/README.md)
1. Conclusion - Suggested tools and resources

## 📚 References

"If I have seen further it is by standing on ye sholders of Giants." -- Sir Isaac Newton

- [Django's Testing Documentation](https://docs.djangoproject.com/en/2.1/topics/testing/)

## 🧠 Resources

- [Testing in Django](https://docs.djangoproject.com/en/2.1/topics/testing/)
- [Edge - Django Boilerplate](https://django-edge.readthedocs.io)

## 🦄 Additional Resources

- [Percy.io - Visual Testing as a Service](https://percy.io/)
- [Travis CI - Hosted CI and CD for GitHub Projects](https://travis-ci.com/)
- [ResembleJS - Image Analysis and Compare Tool](https://huddleeng.github.io/Resemble.js/)
- [Puppeteer - Easy-To-Use NodeJS Library for
  Chrome/Chromium](https://github.com/GoogleChrome/puppeteer)
- [Selenium - Full-Featured Browser Automation](https://www.seleniumhq.org/)

## 🏅 Contributing

Feel free to open an issue or PR. Please read CONTRIBUTING.md for details on the code of conduct,
as well as [PyCon's Code of Conduct](https://us.pycon.org/2019/about/code-of-conduct/).

If you have feedback or questions, you can contact me:

- Email: emily [at] cuttlesoft [dot] com
- Twitter: [@emilyemorehouse](https://twitter.com/emilyemorehouse)
