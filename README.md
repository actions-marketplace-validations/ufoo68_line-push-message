# line-push-message

[![GitHub Actions status](https://github.com/ufoo68/line-push-message/workflows/LINE%20push%20message/badge.svg)](https://github.com/ufoo68/line-push-message/actions)

LINE push message action using GitHub actions

## Usage

* Example

```yml
on: [push]

jobs:
  line_push_message_job:
    runs-on: ubuntu-latest
    name: LINE push message
    steps:
    - name: Push LINE message
      uses: ufoo68/line-push-message@v1.4
      with:
        user-id: ${{ secrets.USER_ID }}
        message: 'test'
        channel-access-token: ${{ secrets.CHANNEL_ACCESS_TOKEN }}
```
