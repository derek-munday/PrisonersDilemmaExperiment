# Code Coverage Instructions

## install environment dependencies

```
sudo apt-get update -qq -y
```
```
sudo apt-get install lcov -y
```
## Run tests and generate report
```
flutter test --coverage
```
```
genhtml coverage/lcov.info -o coverage/html

## Open report
Open the generated html report