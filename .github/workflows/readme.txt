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
    steps:
      # Checks-out your repository under $GITHUB_WORKSPACE, so your job can access it
      - uses: actions/checkout@v2

      # Runs a single command using the runners shell
      - name: Run a one-line script
        run: echo Hello, world!

      # Runs a set of commands using the runners shell
      - name: Run a multi-line script
        run: |
          echo Add other actions to build,
          echo test, and deploy your project.
