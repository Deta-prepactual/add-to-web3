

```yaml
uses: web3-storage/add-to-web3@v2
id: web3
with:
  web3_token: ${{ secrets.WEB3_STORAGE_TOKEN }}
  path_to_add: 'dist'

```

## Inputs

### `path_to_add`

**Required** The path the root directory of your static website or other content that you want to publish to IPFS.

### `web3_token`

**Required** API token for web3.storage

<details>
  <summary>Show advanced options: <code>wrap_with_directory</code>, <code>include_hidden</code>, <code>web3_api</code></summary>

### `wrap_with_directory`


If you do want to capture the `path_to_add` path itself in the IPFS DAG then you want to set `wrap_with_directory:true`.

see: https://web3.storage/docs/reference/js-client-library#parameters

### `include_hidden`

_Default_ `false`

Should hidden files prefixed with a `.` be included when found in the `path_to_add`

see: https://github.com/web3-storage/files-from-path#filesfrompath

### `web3_api`

_Default_ `https://api.web3.storage`

Useful for testing against staging deployments by setting to the api origin of your choice.

</details>



