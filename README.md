# Fighting Game Web Playable Alpha

This public repository contains only a generated browser-playable alpha and
its GitHub Pages deployment workflow. It does not contain the private Engine
source repository, original reference folders, development Replay artifacts or
authoring/debug files.

Like every browser game, the generated `.pck` and WebAssembly payload are
downloaded to each player's browser. They are not the editable source
repository, but they must not be treated as secret or impossible to inspect.

The checked-in `site/` payload keeps large Godot Web files in deterministic
gzip form so every ordinary Git object remains below GitHub's per-file limit.
GitHub Actions restores the ordinary `.pck`, `.wasm` and JavaScript files only
inside the Pages deployment artifact.

This is an early test build. Controls and behavior may change.
