# Eruhitsuji/homebrew-tap

Homebrew Tap for [lifetxt](https://github.com/Eruhitsuji/lifetxt).

```sh
brew install Eruhitsuji/tap/lifetxt
```

## Status

This tap is scaffolding for [lifetxt#572](https://github.com/Eruhitsuji/lifetxt/issues/572).
`Formula/lifetxt.rb` is published automatically by lifetxt's own
[`.github/workflows/homebrew-tap.yml`](https://github.com/Eruhitsuji/lifetxt/blob/main/.github/workflows/homebrew-tap.yml)
whenever a GitHub Release is published there with standalone macOS binaries
attached (see [lifetxt#570](https://github.com/Eruhitsuji/lifetxt/issues/570)).

Until the first such release exists, this tap has no installable Formula.

## Design

`Formula/lifetxt.rb` is a thin adapter around lifetxt's own canonical
standalone-binary release artifacts — it does not build lifetxt from source
or duplicate any of its application logic. See
[docs/en/distribution.md](https://github.com/Eruhitsuji/lifetxt/blob/main/docs/en/distribution.md)
in the main repository for the full distribution architecture.

## Maintenance

- The Formula is regenerated and pushed here automatically on every lifetxt
  release; do not hand-edit `Formula/lifetxt.rb`.
- Formula generation logic lives in
  [`scripts/generate_homebrew_formula.py`](https://github.com/Eruhitsuji/lifetxt/blob/main/scripts/generate_homebrew_formula.py)
  in the main lifetxt repository.
- Issues with lifetxt itself belong in the
  [main repository's issue tracker](https://github.com/Eruhitsuji/lifetxt/issues),
  not here.
