# LAB 4

```
aws lambda create-function --function-name createUpdateFunction ^
--handler createupdate.Handler ^
--runtime java11 ^
--memory 300 ^
--timeout 60 ^
--role "%roleArn%" ^
--environment Variables="{TABLE_NAME=Notes}" ^
--zip-file fileb://createupdateFunction.jar
```