# Heroku

the various ways you could use Heroku to implement a CI solution.

1. Professional workflow in seconds
Organize your pipeline by connecting your GitHub repo, and then automatically or manually placing your Heroku apps in dev, staging or production environments. Simultaneously develop features on dev branches that are reflected by disposable review apps, run tests on every push to GitHub with Heroku CI, merge pull requests, auto deploy to staging, and control who promotes to production.

2. Complete visualization of code delivery
Always know where a particular feature is on the path to production with the real-time Pipelines overview in the Heroku Dashboard. The Pipelines overview provides a single page view of the current relationships between apps, giving your team the state of development across all your environments. With Heroku CI you can see every test run resulting from a push to GitHub.

3. Better quality, tighter iterations
For every open Pull Request, Heroku can spin up a complete disposable environment called a Review App on a unique URL. Every push to a branch in GitHub triggers Heroku CI to run tests. Now everyone can contribute to feature testing early in the product life cycle for speedier decisions and better quality. You can keep staging and production environments identical to catch flaws before your users do.

4. Faster releases, easy collaboration
When combined with Heroku Pipelines, Review Apps and GitHub Integration, Heroku Teams and ChatOps make it even easier to embrace continuous delivery. With Heroku Teams members with the right permissions can collaborate on changes within a Pipeline. Heroku ChatOps makes communication much easier by posting notifications of code changes and deployments associated with a Pipeline in Slack. Team members can see Heroku CI results, deploy to apps in a pipeline, and much more from Slack.

Describe where the various technologies Heroku has to offer fit into each of the testing environments.

You can configure your Heroku CI test environment by including an app.json manifest in your repository’s root directory. During CI test runs, any keys defined in this file’s test environment take precedence over any matching keys in your app’s base configuration. your app or any of its add-ons require certain environment variables during test runs, you can specify them with the env key. te that unlike review apps, Heroku CI does not inherit any config vars from the parent app.To set confidential or volatile environment variables (such as access tokens) that you shouldn’t include in app.json, you can instead add them to your pipeline’s Heroku CI settings in the Heroku Dashboard

Document a possible approach on how to use it for your next "online game project".

One of the reasons Heroku is easy for people to use is that it relies on a widely used revision control system—that is, a way of managing the program code for your app—called Git. In fact, you can’t deploy an app on Heroku unless you are using Git to manage your app clode. The “push” command, “Heroku push master,” is what you input on the command line to send the app from your repository to the cloud. That’s why Heroku is considered a “one click” deploy. It’s not just your own Heroku app that Git makes simple, but any finished app you might encounter on GitHub. Earlier this year, Heroku and GitHub teamed up to create a one click deploy button for repositories on GitHub. So if you see an app you’re interested in learning more about, you can click the deploy button and try it for yourself on Heroku.
