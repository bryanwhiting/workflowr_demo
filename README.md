# workflowr_demo
A quick demo on how to launch workflowr.

# How to Create this Demo
https://jdblischak.github.io/workflowr/#quick-start 

#
1. Create GH repo, clone locally
2. cd into repo
3. `workflowr::wflow_start(directory='.', existing=T)`
4. `workflowr::wflow_build()`
5. `git push`
6. On GitHub > Settings > Options > GitHub Pages > `master docs/`.

Then the site is live.

Configure the [`workflowr report`](https://jdblischak.github.io/workflowr/articles/wflow-05-faq.html#how-can-i-suppress-the-workflowr-report)
1. Add `suppress_report: TRUE` to `_workflowr.yml`
1. Set `suppress_report: false` for `license.Rmd` to have the report available in one place.
1. `wflow_publish("_workflowr.yml", republish = TRUE)`


Add a new analysis:

```
wflow_open('analysis/test_html_widgets.Rmd')
```

Add Google Analytics Measurement ID.
1. Google Analytics > lower left corner > Admin > do a bunch of stuff until you create a new stream.
