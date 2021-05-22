# Changes May 21, 2021 11:00 PM - 11:54 PM
## This forked repository does not deploy to GH Pages <3
- Included the default Jekyll `Gemfile` to properly run (`bundle exec jekyll serve --incremental`) Jekyll locally.
- Created a pull request template in `.github/pull_request_template.md` to strengthen control over collaborative changes towards Collection creation, design changes, development implementations.
- Restructured the post permalinks to remove the date and the file extension. The dates are irrelevant to a literary magazine that publishes posts in Collections and a shorter permalink makes it easier to remember and share amongst each other. Removing the file extension hides the implementation details and makes the URLs more professional.
- Included a 404 Page Not Found page to address the change to permalinks :)
  - 404 Pages can show something humorous and it's open to design ideas
- **IMPORTANT: .gitignore** I included a `.gitignore` file that contains the default Jekyll gitignore for the following reasons:
  - _site is what actually gets deployed and is what you see on the website. GH Pages automatically integrates Jekyll into its build workflow, so _site is generated within GitHub's server. Jekyll's website even recommends ignoring this folder. In addition, _site is just a copy of all the files but in a final website-readable format so it basically doubles the size of the repository due to creating a second copy of every image.
  - caches are only for local deployment and have no impact on the final website.
  - vendor, while not usually on a Jekyll site, might appear if someone attempts to run `gem install`. It's used to locally install gems, so it has no impact on the final website.

- Even prior to permalinks being removed, Jekyll was giving a warning about two similarly named posts. `2020-04-03-skin.md` and `2020-04-06-skin.md` displayed a warning shown in the screenshot below. To address this with the new permalink style, I included the author's last name to the post title, but I can change it to `title-firstName-lastName` if you'd like.

![image](https://user-images.githubusercontent.com/60748722/119217250-d6183d80-ba8d-11eb-9eda-78771406b804.png)

## Future Changes
- I plan on including some Jekyll plugins that improve search engine ranking (SEO) and a sitemap (also for SEO) when I have more free time.