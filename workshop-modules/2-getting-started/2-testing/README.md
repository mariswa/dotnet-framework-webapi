# Testing Existing Catalog API
Your AWS account should now have its own instance of the existing Catalog API. Let's verify that it's working.

## Finding the API's URL
Click [here](https://console.aws.amazon.com/elasticbeanstalk/home#/application/overview?applicationName=stackery-demo-dotnet-framework-api) to open the Elastic Beanstalk console for the Catalog API. If you don't see the application, make sure you are logged into in the correct AWS account and region for this workshop.

![Elastic Beanstalk Console](./ebconsole.png)

Now click the **URL** link for the *production* environment. It will first take you to an error page, which is expected.

![Error Page](./rooterror.png)

## Querying for Books
In your browser's URL bar add `/api/books` to the end and hit *enter*. You should see the following page result:

![Books Records](./books.png)

> The first time you navigate to this page it may take up to 30 seconds to respond. The server does a bunch of initialization during the first request, including migrating and seeding the database.

You are now ready to continue onto the [Workshop Setup](../../3-workshop-setup/README.md)!