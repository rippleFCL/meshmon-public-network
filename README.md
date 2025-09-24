# meshmon-public-network

## How to PR Your Own Node

1. **Fork this repository** to your own GitHub account.
2. **Edit `config.yml`**:
	 - Add a new entry under `node_config` for your node. Example:
		 ```yaml
        - node_id: yourname
           poll_rate: 30
           retry: 2
           url: https://your-node-url.com # optional if your node is publicly exposed
		 ```
	 - Make sure your `node_id` is unique.
	 - Set `url` to your node's public endpoint.
3. **Add your public key** to the `pubkeys/` directory as `yourname.pub`.
4. **Commit and push** your changes to your fork.
5. **Open a Pull Request** to this repository's `main` branch.
6. Wait for review and approval.

That's it! Once approved, your node will be part of the meshmon public network.
