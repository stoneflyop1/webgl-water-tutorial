# WebGL Basic Water Tutorial

If you have any questions or run into any stumbling blocks please feel free to
[open an issue](https://github.com/chinedufn/webgl-water-tutorial/issues)!

[Read the tutorial](http://chinedufn.com/3d-webgl-basic-water-tutorial/)

![Screenshot of tutorial](/screenshot.png)

```sh
# You can use any static file server that properly sets the
# `application/wasm` mime type
npm install -g http-server

git clone https://github.com/chinedufn/webgl-water-tutorial
cd webgl-water-tutorial
cargo install -f wasm-bindgen@0.2.29 # Or download a release binary
./build.sh

## Opens your browser to http://localhost:8080  where the demo will be running
http-server --open
```

or you can use `wasm-pack` and python3's simple httpserver module

``` sh
wasm-pack build --target no-modules
cp pkg/webgl_water_tutorial.js ./
cp pkg/webgl_water_tutorial_bg.wasm ./
python3 server.py # http://localhost:8000
```

# See Also

- [ThinMatrix's OpenGL Water Tutorial](https://www.youtube.com/watch?v=HusvGeEDU_U&list=PLRIWtICgwaX23jiqVByUs0bqhnalNTNZh) - Heavily inspired this WebGL implementation
- [Landon](https://github.com/chinedufn/landon) - Used for exporting meshes and armatures from Blender
