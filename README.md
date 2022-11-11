

# install-pinned/ruff

![](https://shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)

Securely install the latest [ruff](https://pypi.org/project/ruff/) release from PyPI.

This action installs a pinned version of **ruff** and all its dependencies,         making sure that file hashes match. Pinning your dependencies stops supply chain attacks where an adversary         replaces ruff or one of its dependencies with malicious code.

## Usage

In your GitHub Actions workflow, use this action like so:

```yaml
      - name: Install ruff from PyPI
        uses: install-pinned/ruff@a91fd0bb1e3810cfb40c18d788234e2d2b1d2335  # 0.0.110
```

## Alternatives

This action is a relatively simple wrapper around the fantastic [pip-tools](https://pip-tools.rtfd.io)         and is most useful if there is no existing `requirements.txt`/`poetry.lock`/... infrastructure in place.         If you already pin all your dependencies in a single place, you don't need it!

## More Details

See the [@install-pinned README](https://github.com/install-pinned) for details.
