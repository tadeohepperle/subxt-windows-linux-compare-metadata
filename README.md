how the hex, scale and json files where generated on windows and linux:

```
subxt metadata --url wss://rpc.polkadot.io:443 -f hex > polkadot_remote_windows.hex
subxt metadata --url wss://rpc.polkadot.io:443 -f bytes > polkadot_remote_windows.scale
subxt metadata --url wss://rpc.polkadot.io:443 -f json > polkadot_remote_windows.json

subxt metadata --url wss://rpc.polkadot.io:443 -f hex > polkadot_remote_linux.hex
subxt metadata --url wss://rpc.polkadot.io:443 -f bytes > polkadot_remote_linux.scale
subxt metadata --url wss://rpc.polkadot.io:443 -f json > polkadot_remote_linux.json
```


```
subxt metadata --file ../subxt/artifacts/polkadot_metadata_tiny.scale -f hex > polkadot_tiny_windows.hex
subxt metadata --file ../subxt/artifacts/polkadot_metadata_tiny.scale -f bytes > polkadot_tiny_windows.scale
subxt metadata --file ../subxt/artifacts/polkadot_metadata_tiny.scale -f json > polkadot_tiny_windows.json

subxt metadata --file ../subxt/artifacts/polkadot_metadata_tiny.scale -f hex > polkadot_tiny_linux.hex
subxt metadata --file ../subxt/artifacts/polkadot_metadata_tiny.scale -f bytes > polkadot_tiny_linux.scale
subxt metadata --file ../subxt/artifacts/polkadot_metadata_tiny.scale -f json > polkadot_tiny_linux.json
```

how the scale_hexdump files were generated:

```
<./polkadot_lin.scale | hexdump > polkadot_lin.scale_hexdump
<./polkadot_win.scale | hexdump > polkadot_win.scale_hexdump


<./polkadot_tiny_windows.scale | hexdump > polkadot_tiny_windows.scale_hexdump
<./polkadot_tiny_linux.scale | hexdump > polkadot_tiny_linux.scale_hexdump
```
