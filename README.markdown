# The differences between `rails new` with flags.

In this repository, you can see the difference in the output code when `rails new` is given a flag such as `-skip-javascript`.

Note that obvious flags such as `-ski-bundle` and `-skip-gemfile` are not covered.

## Summary

Click 🔍 to see the differences with no flags.

| flag | 6.0.4.4 | 6.1.4.4 | 7.0.1 |
| --- | --- | --- | --- |
| --api | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-api) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-api) | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-api) |
| --asset-pipeline=propshaft | - | - | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-asset-pipeline-propshaft) |
| --asset-pipeline=sprockets | - | - | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-asset-pipeline-sprockets) |
| --css=bootstrap | - | - | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-css-bootstrap) |
| --css=bulma | - | - | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-css-bulma) |
| --css=postcss | - | - | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-css-postcss) |
| --css=sass | - | - | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-css-sass) |
| --css=tailwind | - | - | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-css-tailwind) |
| --javascript=esbuild | - | - | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-javascript-esbuild) |
| --javascript=importmap | - | - | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-javascript-importmap) |
| --javascript=rollup | - | - | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-javascript-rollup) |
| --javascript=webpack | - | - | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-javascript-webpack) |
| --minimal | - | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-minimal) | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-minimal) |
| --skip-action-cable | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-action-cable) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-action-cable) | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-skip-action-cable) |
| --skip-action-mailbox | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-action-mailbox) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-action-mailbox) | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-skip-action-mailbox) |
| --skip-action-mailer | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-action-mailer) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-action-mailer) | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-skip-action-mailer) |
| --skip-action-text | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-action-text) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-action-text) | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-skip-action-text) |
| --skip-active-job | - | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-active-job) | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-skip-active-job) |
| --skip-active-record | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-active-record) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-active-record) | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-skip-active-record) |
| --skip-active-storage | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-active-storage) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-active-storage) | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-skip-active-storage) |
| --skip-asset-pipeline | - | - | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-skip-asset-pipeline) |
| --skip-bootsnap | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-bootsnap) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-bootsnap) | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-skip-bootsnap) |
| --skip-hotwire | - | - | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-skip-hotwire) |
| --skip-javascript | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-javascript) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-javascript) | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-skip-javascript) |
| --skip-jbuilder | - | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-jbuilder) | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-skip-jbuilder) |
| --skip-listen | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-listen) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-listen) | - |
| --skip-puma | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-puma) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-puma) | - |
| --skip-spring | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-spring) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-spring) | - |
| --skip-sprockets | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-sprockets) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-sprockets) | - |
| --skip-system-test | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-system-test) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-system-test) | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-skip-system-test) |
| --skip-test | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-test) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-test) | [🔍](https://github.com/snaka/rails_new_flags/compare/7.0.1..7.0.1-skip-test) |
| --skip-turbolinks | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-skip-turbolinks) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-skip-turbolinks) | - |
| --webpacker | [🔍](https://github.com/snaka/rails_new_flags/compare/6.0.4.4..6.0.4.4-webpacker) | [🔍](https://github.com/snaka/rails_new_flags/compare/6.1.4.4..6.1.4.4-webpacker) | - |
