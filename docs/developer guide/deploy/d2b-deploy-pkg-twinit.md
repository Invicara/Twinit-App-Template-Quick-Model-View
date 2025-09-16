[Gather Necessary Info and Check Twinit Access](./d1-gather.md) < Back | **Next** > [Build and Run the Web Client](./d3-webclient.md)

---

# Deploy Step 2: Use a Template Package to Deploy the Application Template to Twinit

> Note: In order to use Template Packages to deploy the Quick Model View Application Template you must be using the Twinit Visual Studio Code Extension version 7.0.0 or later.

Next you will deploy the template and its configuration to Twinit. This is the first of two deploys to completely deploy the template. In a later step you will learn how to build and deploy the template's web client.

> Note: Images are provided as an example of what you will see during the deployment process. Depending on the release of Quick Model View which you are deploying, the actual scripts and configs you see will differ

To deploy the template to Twinit you will:

1. Clone/Fork the template code locally
2. Sign in to Twinit and your application using the Twinit VSCode Extension
3. Create a new "Quick Model View Manager" project for your application
4. Use a Template Package to deploy all the code and configuration for the template to your Twinit project

Remember, as mentioned in the [General Introduction](../implementation/general-intro.md), what you are setting up now is the ability to create new Quick Model View projects, not actually creating new Quick Model View projects themselves.

## Clone or Fork the Quick Model View 

1. Using your preferred github method, clone or fork this repository locally

## Sign in to Your Application using the Twinit VS Code Extension

1. Sign in to Twinit using the Twinit VS Code extension
2. Select the Twinit instance in which you be working when prompted
3. Select your application when prompted

Your Twinit extension panel should look like this, with your application name displayed.

```
TWINIT
├─ Quick Model View
```

## Create a New "Quick Model View Manager" project

1. Right click on your application name in the Twinit extension and select "New Project"
2. Enter "QMV Manager" when prompted for a project name
3. Enter "QMV Manager" when prompted for a project description
4. Enter "qmvman" when prompted for a project short name

A new project should now be visible in the extension panel.

```
TWINIT
├─ Quick Model View
│  ├─ QMV Manager (p)
```

## Deploy the Template Package

1. Expand your new "QMV Manager" project in the extension panel
2. Right click on the Project folder and select "Deploy Template Package"
3. When prompted to select a template package select ```setup/template packages/Quick Model View Maager.zip```

The project will then be deployed with the contents of the template package. When complete the results of the deploy log will display and your project should show these Scripts and User Configs:

```
TWINIT
├─ Quick Model View
│  ├─ QMV Manager (p)
│  │  ├─ Scripts
│  │  │  ├─ [v1] importHelperTemplate (quick-temp) <b>
│  │  │  ├─ [v1] mapboxTemplate (quick-temp) <b>
│  │  │  ├─ [v1] Project Maker (project-maker)
│  │  ├─ User Configs
│  │  │  ├─ [v1] QuickViewAdminConfigTemplate (quick-temp)
│  │  │  ├─ [v1] QuickViewManagerConfig (quick-view)
│  │  │  ├─ [v1] QuickViewViewerConfigTemplate (quick-temp)
│  │  ├─ API Configs
```

## Next Steps

In the previous steps you deployed the Quick Model View Manager configuration and scripts to Twinit along with the template script and user configurations it needs to create new Quick Model View projects.

In the next step you will build and run the template web client.

---
[Gather Necessary Info and Check Twinit Access](./d1-gather.md) < Back | **Next** > [Build and Run the Web Client](./d3-webclient.md)