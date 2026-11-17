# GLB Viewer

Um visualizador simples de arquivos 3D no formato GLB para web.

Para rodar o projeto:

```
npx serve
```

## Pasta `vendor/`

Os arquivos HTML continuam carregando as dependências via CDN (`esm.sh`, `jsdelivr`, `gstatic` e Google Fonts), mas a pasta `vendor/` guarda uma cópia local de todas elas por precaução — caso algum CDN fique fora do ar, mude versões implicitamente ou seja necessário rodar o projeto offline:

- `vendor/preact/` — `preact@10.19.2` (incluindo `hooks`)
- `vendor/htm/` — `htm@3.1.1` (`htm/preact`)
- `vendor/three/` — `three@0.160.0` (incluindo `examples/jsm/` e `examples/jsm/libs/basis/`)
- `vendor/meshoptimizer/` — `meshoptimizer@0.21.0`
- `vendor/draco/1.5.6/` — decoders Draco (`draco_decoder.js`, `draco_decoder.wasm`, `draco_wasm_wrapper.js`)
- `vendor/fonts/` — fonte `Outfit` (`outfit.css` e arquivos `.woff2`)

## Créditos

Os modelos GLB foram obtidos em:

- [ohzinteractive/glb-viewer-web - public/models](https://github.com/ohzinteractive/glb-viewer-web/tree/main/public/models)
- [mrdoob/three.js - examples/models/gltf](https://github.com/mrdoob/three.js/tree/dev/examples/models/gltf)
