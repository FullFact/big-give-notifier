# Big Give notifier

Sends Slack updates about how the Big Give is going.

## Setup

1. You’ll need to set up a [Slack workflow](https://docs.slack.dev/messaging/sending-messages-using-incoming-webhooks/) that runs on webhook trigger, and sends a message containing the data it receives
2. You’ll need to add the trigger URL as a repo secret called `SLACK_TRIGGER_URL`
3. Add the Big Give campaign ID as a repo variable called `BIG_GIVE_CAMPAIGN_ID`
4. Uncomment the schedule stuff in the GitHub workflow


## Format code

```
ruff check --select I . --fix
ruff format .
```