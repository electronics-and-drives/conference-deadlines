## Conference Deadlines 

Countdown timers to keep track of conference deadlines around the interests of
[Electronics & Drives](https://www.electronics-and-drives).

This is a fork of [ai-deadlines](https://github.com/paperswithcode/ai-deadlines),
all credit goes to them.

## Contributing

To add or update a deadline:
- E&D members clone the repository, others fork the repository 
- Update `_data/conferences.yml`
- Make sure it has the `title`, `year`, `id`, `link`, `deadline`, `timezone`,
  `date`, `place`, `sub` attributes
    + See available timezone strings [here](https://momentjs.com/timezone/).
- Optionally add a `note` and `abstract_deadline` in case the conference has a
  separate mandatory abstract deadline
- Optionally add `hindex` (refers to h5-index from
  [here](https://scholar.google.com/citations?view_op=top_venues&vq=eng))
- Example:
    ```yaml
    - title:             EDAC
      year:              2026
      id:                edac26                 # title as lower case + last two digits of year
      full_name:         Best EDA Conference    # full conference name
      link:              link-to-website.com
      deadline:          YYYY-MM-DD HH:SS
      abstract_deadline: YYYY-MM-DD HH:SS
      timezone:          UTC+1
      place:             Munich, Germany
      date:              September, 18-22, 2026 # In plain text
      start:             YYYY-MM-DD
      end:               YYYY-MM-DD
      paperslink:        link-to-full-paper-list.com
      hindex:            13
      sub:               EDA
      note:              Call for papers, etc.
    ```
- E&D members just push, others send a pull request

## Test Locally

Refer to [GitHub Pages Guide](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll)

```
$ bundle install
$ bundle exec jekyll build
$ bundle exec jekyll serve
```

## Known Issues

- [ ] Multiple `sub` causes black color in calendar [original PR](https://github.com/paperswithcode/ai-deadlines/pull/293)
- [ ] No Notification Date ([yet](https://github.com/paperswithcode/ai-deadlines/issues/388))
