# Looking for easy tasks for Hacktoberfest?

<img width="640" height="439" alt="image" src="https://github.com/user-attachments/assets/719fe876-946f-4c36-969e-970a8e929935" />

We scanned open-source repos and found a bunch of easy-to-fix items: hacks and "temporary" workarounds compensating for upstream bugs. These aren’t feature work, but rather low-risk cleanups that remove technical debt and make open source projects easier to maintain. 

For example: one repo included this workaround comment:

```
# The SDK requires the first message to be a user message 
# This is not the case if user used `start_conversation` 
# Workaround from https://github.com/googleapis/python-genai/issues/529#issuecomment-2740964537
```

The linked issue was a regression that’s been fixed upstream, so the workaround could possibly be removed (after verifying the fixed version of the dependency is in use). 

These tasks are ideal for Hacktoberfest contributors who want quick, easily reviewable PRs that actually help maintainers.

| Issue | Referenced in [repo/path/to/file:line] |
| --- | --- |
|https://github.com/stretchr/testify/issues/497 | [anchore/syft/internal/file /zip_file_traversal_test.go:241](https://github.com/anchore/syft/blob/675075e8828d04090ec6bf4a566542bf1dec019f/internal/file/zip_file_traversal_test.go#L241) | 
| https://github.com/anchore/syft/issues/1837 | [syft/syft/license/license.go:34](https://github.com/anchore/syft/blob/675075e8828d04090ec6bf4a566542bf1dec019f/syft/license/license.go#L34) |
| https://github.com/googleapis/python-genai/issues/529 | [core/homeassistant/components/google_generative_ai_conversation/entity.py:536](https://github.com/home-assistant/core/blame/23e7b14eae718b75f3e406f95e5fbcc4403b510f/homeassistant/components/google_generative_ai_conversation/entity.py#L536) |
| https://github.com/gcobb321/icloud3/issues/349 | [homeassistant/loader.py:108](https://github.com/home-assistant/core/blob/6a1cf9827cc735574da664faa97000481f1d6770/homeassistant/loader.py#L108) |
| https://github.com/forem/forem/issues/14100 | [forem/app/javascript/modCenter/singleArticle/__tests__ /singleArticle.test.jsx:23](https://github.com/forem/forem/blob/8220a68668d78577050ab14d311779dbeace48fc/app/javascript/modCenter/singleArticle/__tests__/singleArticle.test.jsx#L23) |
| https://github.com/rust-lang/cargo/issues/15080 | [bat/build /syntax_mapping.rs:241](https://github.com/sharkdp/bat/blob/4e13c3eb5bd5e78de8cafb4b21f646b880216c2d/build/syntax_mapping.rs#L241) | 

This list was generated with [HackStalker](https://hackstalker.dev/) (beta), a lightweight quality assurance tool that scans codebases for references to GitHub issues and temporary hacks, tracks upstream bugs, and alerts you when it’s safe to remove a workaround. We’re actively developing it, so please try it, report bugs, or request features. Your [feedback](https://github.com/hack-stalker/community/discussions/) will directly shape the tool.

Happy hacking!
