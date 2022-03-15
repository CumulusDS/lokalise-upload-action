[![Create Release][release-badge]][release-url]
[![Import Labels][import-labels-badge]][import-labels-url]
[![Sync Labels][sync-labels-badge]][sync-labels-url]
[![PR AutoLabeler][autolabeler-badge]][autolabeler-url]
[![Assigner][assigner-badge]][assigner-url]

Extracts language internationalization & uploads to Lokalise

### Inputs
#### `token`
Your CLI/API token for Lokalise
Required.

#### `projectId`
Your Lokalise project ID
Required.

#### `filePath`
The path to the file(s) you want to upload to Lokalise
Not required.
Default: `lang`

#### `npmToken`
Token used for NPM authentication
Required

#### `nodeVersion`
What node version to install
Not required.
Default: `12`


### Example usage
```yaml
      - name: Lokalise upload
        uses: CumulusDS/lokalise-upload-action@v1
        with:
          token: ${{ secrets.TOKEN_FOR_LOKALISE }}
          projectId: ${{ secrets.PROJECT_ID }}
          filePath: lang
```


[release-badge]: https://github.com/CumulusDS/lokalise-upload-action/actions/workflows/release.yml/badge.svg
[release-url]: https://github.com/CumulusDS/lokalise-upload-action/actions/workflows/release.yml
[import-labels-badge]: https://github.com/CumulusDS/lokalise-upload-action/actions/workflows/labels_import.yml/badge.svg
[import-labels-url]: https://github.com/CumulusDS/lokalise-upload-action/actions/workflows/labels_import.yml
[sync-labels-badge]: https://github.com/CumulusDS/lokalise-upload-action/actions/workflows/labels_sync.yml/badge.svg
[sync-labels-url]: https://github.com/CumulusDS/lokalise-upload-action/actions/workflows/labels_sync.yml
[autolabeler-badge]: https://github.com/CumulusDS/lokalise-upload-action/actions/workflows/autolabeler.yml/badge.svg
[autolabeler-url]: https://github.com/CumulusDS/lokalise-upload-action/actions/workflows/autolabeler.yml
[assigner-badge]: https://github.com/CumulusDS/lokalise-upload-action/actions/workflows/assign.yml/badge.svg
[assigner-url]: https://github.com/CumulusDS/lokalise-upload-action/actions/workflows/assign.yml
