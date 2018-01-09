# test-serilog-cf
Example Project for configuring serilog to use compact, structured JSON logs

## Areas of Interest
Check out the test-logging.csproj file to see the referenced packages this example uses.  Also check out Program.cs for the initialization and configuration for Serilog.

## Testing this out
Clone this repo locally to test out logging with Serilog

### Running on CloudFoundry
In a terminal from the root of the cloned repo:
1. Call `cf push test-serilog` to push and start the example app.
2. Call `cf logs test-serilog` to tail the logs for the app.
3. After the app is started, open a browser and go to the URL bound to your application (you can see it in the output of the push command at the end).  This will generate an exeception which you can see in the terminal.

### Running locally
In a terminal from the root of the cloned repo:
1. Call `dotnet restore` to retrieve all the dependencies.
2. Call `dotnet run` to run the app locally.
3. After the app is started, open a browser and go to the host and port your application is started under (you can see that info in the terminal output at the end).  This will generate an exeception which you can see in the terminal.
