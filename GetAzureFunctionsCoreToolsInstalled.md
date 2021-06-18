// install chocolaty
// run this in a command line
@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "[System.Net.ServicePointManager]::SecurityProtocol = 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"

//to test run choco at the cmd

Install the .NET Core SDK version 2.1 using the following command:
// change version as need be
choco install dotnetcore-sdk --version=2.1.502 -y

Check that .NET Core SDK is installed properly by opening a new command prompt and running the following command:

dotnet --version
Now install NodeJS using choco:

choco install nodejs-lts -y --force
Open a new administrative command prompt and install Azure Functions Core Tools using the following command:

npm i -g azure-functions-core-tools@3 --unsafe-perm true

