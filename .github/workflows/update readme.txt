name: Greeting from Patrick Yung
on: push
jobs:
  my-job:
    Name: My Job
    run-on: ubuntun-latest
    steps:
    - name: Print a greeting
    env:
        MY_VAR: Hi there! My name is 
        FIRST_NAME: Pak Hong
        MIDDLE_NAME: Patrick
        LAST_NAME: Yung
        
    run:
      echo $MY_VAR $FIRST_NAME $MIDDLE_NAME $LAST_NAME.
