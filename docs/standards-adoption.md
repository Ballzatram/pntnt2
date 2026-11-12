# Engineering standards adoption

Owner: Ballzatram. Policy: 1.0.0. Baseline source revision: `554bb4f59a06bbe20d2d4bad805d49a53f7657e4`.

Static art/music site: four routes, canvas veil and persistent pane navigation. Preserve artwork, route names, storage keys and interaction behavior.

## Verification

Run `uv run --project .engineering --locked python .engineering/tools/audit.py .` for structural prerequisites. Existing native test/build commands are retained in README and the workflows. `.github/workflows/engineering.yml` adds a consistent, read-only verification gate; it never deploys or uses production secrets. Review `docs/audit.md` for controls requiring manual evidence.

The command register includes existing syntax/compile checks where no full static type checker exists; these are not equivalent to strict typing. Legacy formatter/type/coverage gaps remain explicit, not silently waived. No approved exceptions have been invented. Source import/native platform requirements and hosted protections must be reviewed separately.

## Preservation

Default branches and deployed services are not changed by preparing this branch. Runtime source changes, if any, are limited to documented regression fixes and must pass the existing tests. Do not run live research, mail, payment, model generation, customer data changes or production deployment as a standards check.

## Recorded local verification

The route/resource/script contract passes for all four pages. Application HTML/CSS/JavaScript is unchanged. The separate dirty local checkout was not modified.

See docs/audit.md for unresolved controls. A structural pass is not full conformance.

## Final candidate checks

See [merge verification](merge-verification.md) for current gates, commands and actual performance/coverage measurements. This supersedes the initial local-only/native-pending notes above. See .standards.json for the executable command register. Hosted feature restrictions and remaining conformance work remain explicit.
