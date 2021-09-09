The sample app is located here: [Embedded Sign-In Widget sample app](https://github.com/okta/samples-golang/tree/master/identity-engine/embedded-sign-in-widget).

## Steps to test the sample app

1. Ensure that you've configured your Okta org properly by completing the steps in [Set up your Okta org (for password factor only use cases)](/docs/guides/oie-embedded-common-org-setup/go/main/#set-up-your-okta-org-for-password-factor-only-use-cases).
1. Ensure you've completed the steps in [download and set up the sample app](/docs/guides/oie-embedded-common-download-setup-app/go/main/).
1. Open the embedded Widget sample application directory using Visual Studio Code or
   your preferred IDE. The directory path to the sample application directory is: `samples-golang/identity-engine/embedded-sign-in-widget`.
1. Add an `okta.yaml` configuration file. See [Option 1: YAML configuration file](/docs/guides/oie-embedded-common-download-setup-app/go/main/#option-1-configuration-file) for more information on how to configure and where to place the configuration file.
1. From the command line, navigate to the Widget's sample application directory (`../samples-golang/identity-engine/embedded-sign-in-widget/`).
1. From the command line, execute the following command to install dependencies: `go get`
1. From the command line, execute the following command to start the application: `go run main.go`
1. In a web browser, navigate to `http://localhost:8000/`. The Go embedded Widget app landing page appears:

   <div class="common-image-format">

    ![The home page of the Golang Widget sample application](/img/oie-embedded-sdk/oie-embedded-widget-golang-sample-app-home-page.png)

   </div>

1. Click **Login**.
1. On the sign-in page enter the username (email) and password that you've used in
[Create your Okta account](/docs/guides/oie-embedded-common-org-setup/go/main/#create-your-okta-account).
1. If you've successfully signed in, the following screen is displayed
   with the user name:

   <div class="common-image-format">

    ![The default page showing the user profile information](/img/oie-embedded-sdk/oie-embedded-widget-golang-sample-app-user-default-page.png)

   </div>

## Troubleshooting

* If you see the "There was an unexpected internal error. Please try again." message instead of the Sign-In Widget, then verify that CORS is enabled. Follow the steps in [Add a trusted origin and enable CORS](/docs/guides/oie-embedded-common-org-setup/go/main/#step-3-add-a-trusted-origin-and-enable-cors) to enable CORS.