# PCF Text Control Input

Standard text input control for Power Apps model driven apps. Built as part of [this](https://ryanspain.net/posts/build-a-pcf-text-control/) blog post.

![Text input control](img/preview.gif?raw=true)

## Build the PCF control

Install the required NPM packages, and build the control by executing the following command from **📁src/project**.

```cmd
npm install
```

```cmd
npm run build
```

## Test the PCF control

From **📁src/project**, execute the below command to build the control and start the test harness.

```cmd
npm run start
```

## Build the CDS solution

From the **📁src/solution** folder, run the following command.

```cmd
msbuild /t:build /restore
```

For subsequent builds, use the following command.

```cmd
msbuild /t:rebuild
```

The importable solution files can be found in **📁bin/Debug**.

## Deploy

Import the solution generated in the previous step into your environment.

## Configure

Follow this [documentation](https://docs.microsoft.com/en-us/powerapps/developer/component-framework/add-custom-controls-to-a-field-or-entity#add-a-code-component-to-a-field) to configure the control on a field.
