# org-actions-provision-runner

GitHub Action to provision GitHub Actions runner with security tools.

## Usage

Use this action as the first step in your workflows, and ensure it's passed the required secrets.
You will also need to use this action in any reusable workflows and pass secrets down from the
calling action.

```yaml
      - name: Provision runner
        uses: nationalarchives/org-actions-provision-runner@73234518dd1d4206c78c325fc4765bf4467eb71f # v1.0.0
        with:
          wiz-sensor-token: ${{ secrets.WIZ_SENSOR_TOKEN }}
```