# get the necessary cargo stuff
cargo install wasm-pack

# make a new rust project and do your code
cargo init --lib

# make the package
wasm-pack build

# get the necessary npm stuff
npm install

# bundle everything
node_modules/.bin/webpack

# start the server
cd dist; ../node_modules/.bin/wasm-server

# go to http://127.0.0.1:3000