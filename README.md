# Slack Build Notification Action

This action sends a notification to a Slack channel about the application build status.

## Usage

```yaml
steps:
  - name: Build Android bundle
    uses: AcmeSoftwareLLC/slack-build-notification@v1
    with:
      platform: android
      webhook-url: ${{ secrets.SLACK_WEBHOOK_URL }}
      build-name: 1.0.0
      build-number: 20231005
      changelog: |
        ## Changelog
        - Added new feature
        - Fixed bug
```
