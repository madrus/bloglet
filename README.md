# Creating my blog with Jekyll on GitHub Pages

> Blog link: [https://madrus.github.io/bloglet][1]

For my theme, I have taken the [Lanyon Theme][2]. And here is its [source code link][3]. I have also found a very nice tutorial how to begin with it:  [GitHub Pages and Jekyll Beginner Video][4]. I have also decided to keep the original three posts of __Mark Otto__ [@mdo](https://twitter.com/mdo) in my blog as an honor to his work and as an introduction to his theme.

## Deployment to GitHub Pages

[GitHub Pages](https://pages.github.com/) are freely hosted by `GitHub` on its `github.io`. My personal page is [madrus.github.io](https://madrus.github.io).

### Steps to take

*   run the blog locally: `bundle exec jekyll serve`
*   create a new `gh-pages` branch: `git branch gh-pages`
*   push `master` and `gh-pages` branches to `GitHub`
*   the blog will be available at [https://madrus.github.io/bloglet][1]
*   If we want to our blog to be available at our own domain, we can add `CNAME` file in the root with just the `URL`, e.g.:

    ```
    myblogurl.com
    ```

    As soon as we commit the file to the `gh-pages` repository and push it to `GitHub`, we can navigate to [myblogurl.com](http://myblogurl.com) to see our blog.

    *   `git add .`
    *   `git commit -am "cname added"`
    *   `git push -u origin master`
    *   `git checkout gh-pages`
    *   `git merge master`
    *   `git push -u origin gh-pages`



[1]: https://madrus.github.io/bloglet
[2]: http://lanyon.getpoole.com/
[3]: https://github.com/poole/lanyon
[4]: https://www.youtube.com/watch?v=T2nx6tj-ZH4
