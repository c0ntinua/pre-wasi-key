![Screenshot 2023-01-14 at 5 07 55 AM](https://user-images.githubusercontent.com/90075803/212466978-4755b046-a3c5-493d-9b58-17341d48bafe.png)
# pre-wasi-key

This program is especially intended for WebAssembly runtimes. It creates a random key for the symmetric crypto system 'pre.' This is implemented in Go elsewhere in this repo, but I am currently working on the Rust version, this time separating key-creation from encryption/decryption. The screen above features the first working version. After giving access to the working directory, you can follow positive integer arguments for RANGE INPUT_LENGTH PREFIX_CODE_LENGTH RESPONSES STATES.  The last argument is the alphabet (your prefered symbols for displaying what are actually u8's under the hood.)

For instance, in the screenshot, I used:

`wasmer pre-wasi-gen.wasm --dir=. 3 3 3 3 6 9 'O|@'`
