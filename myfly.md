# install flyctl
If you have the Homebrew package manager installed, flyctl can be installed by running:
brew install flyctl

If not, you can run the install script:
curl -L https://fly.io/install.sh | sh

# init node app
npm init -y
nmp i express

# Run node server.js to start the application
node server.js

# signup
flyctl auth signup

# To launch an app on fly, run flyctl launch in the directory with your source code. This will create and configure a fly app for you by inspecting your source code, then prompt you to deploy.
flyctl launch


# To deploy changes to your app, just run:
flyctl deploy

# Now the application has been deployed, let's find out more about its deployment. The command flyctl info will give you all the essential details.
flyctl status

# The quickest way to browse your newly deployed application is with the flyctl open command.
flyctl open

# If you want to know what IP addresses the app is using, try flyctl ips list:
flyctl ips list
