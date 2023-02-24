## Conference Deadlines 

Countdown timers to keep track of conference deadlines around the interests of
[Electronics & Drives](https://www.electronics-and-drives).

This is a fork of [ai-deadlines](https://github.com/paperswithcode/ai-deadlines),
all credit goes to them.

## Contributing

To add or update a deadline:
- Fork the repository
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
    - title:             EDAConf
      year:              2026
      id:                edaconf26              # title as lower case + last two digits of year
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
      pwclink:           link-to-papers-with-code.com
      hindex:            1.0
      sub:               EDA
      note:              Call for papers, etc.
    ```
- Send a pull request
