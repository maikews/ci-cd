```
name: GitHub Actions
on: [push]
jobs:
  simple-test:
    runs-on: ubuntu-latest
    steps:
      - run: echo "🎉 Start Test"

      - name: Check out repository code
        uses: actions/checkout@v4

      - name: Make the script files executable
        run: chmod +x script.sh

      - name: execute test
        run: ./script.sh
```
