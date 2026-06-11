# Cad0p Tap

Homebrew tap for stable `cad0p` macOS/Homebrew formulae.

Prerelease formulae live in [`cad0p/homebrew-prerelease`](https://github.com/cad0p/homebrew-prerelease).

## Prerequisites

`ghostty-zmx` depends on zmx from the upstream `neurosnap/tap` tap:

```sh
brew tap neurosnap/tap
```

## Formulae

### `ghostty-zmx`

Stable releases of Ghostty + zmx session management integration.

Install the formula directly. This automatically taps the repository and trusts only this formula:

```sh
brew install cad0p/tap/ghostty-zmx
```

After installation, configure your shell and Ghostty config by running:

```sh
ghostty-zmx-install
```

Then restart Ghostty or open a new Ghostty window.

## Manual tap installation

If you want to add the tap without installing a formula immediately:

```sh
brew tap cad0p/tap
```

Then install a formula explicitly:

```sh
brew install cad0p/tap/ghostty-zmx
```

With Homebrew Tap Trust, prefer the fully-qualified `brew install cad0p/tap/<formula>` form when possible. It installs the formula and trusts only that formula.

## Development

Formula files live under `Formula/`:

```text
Formula/ghostty-zmx.rb
```

Before pushing formula changes, test locally:

```sh
brew install --build-from-source cad0p/tap/ghostty-zmx
brew test cad0p/tap/ghostty-zmx
brew audit --strict cad0p/tap/ghostty-zmx
```

## Documentation

`brew help`, `man brew`, or [Homebrew's documentation](https://docs.brew.sh).
