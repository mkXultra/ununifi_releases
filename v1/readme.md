target_branch=feature/listing_and_nft_mint`
cd chain
git checkout $target_branch
make build
cd build
cp ~/go/pkg/mod/github.com/!cosm!wasm/wasmvm@v1.0.0-beta10/api/libwasmvm.so .
tar -zcvf  ununifid-v0.0.1-linux-amd64.tar.gz ./ununifid ./libwasmvm.so


