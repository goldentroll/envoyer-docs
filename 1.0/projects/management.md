# Management

[[toc]]

## Overview

Within Envoyer, your application is represented by a "project". Projects can be deployed to one or more servers at the same time.

## Creating a Project

To create a project, click the **Add Project** button at the top of the Envoyer dashboard. You will be presented with a modal that asks you to provide a few details about the project.

If you don't see the Source Control provider that you need, make sure that you've linked it in your account settings.

Once you've provided the details regarding your project, click **Save Project**.

:::warning Don't see the Add Project button?

Make sure that you've subscribed to one of Envoyer's paid subscriptions.
:::

## Project Settings

To make changes to your project settings, click the **Settings** button at the top of the project's dashboard.

From here, you can change the project settings, source control settings, and delete the project. In addition, you can edit the project's name, type, health check URL, and how many deployments to retain for the project

### Health Checks

When your site has finished deploying, Envoyer can ping it to ensure that it is still available. Health checks are performed from three locations:

- New York
- London
- Singapore

If you have configured notifications on your project, Envoyer will notify these channels of the result of the health check.

:::warning Health Checker Status Codes

The configured URL must return a `2xx` status code. All other status codes will be considered a failure.
:::

### Source Control

You can manage how the project is deployed via the project's source control settings. Specifically, you may configure from which source control provider the project is deployed, the branch that is deployed, and you may also choose whether to install the project's Composer dependencies.

You may also enable the project's **Deploy When Code Is Pushed** setting. Enabling this setting will add a webhook to your source control provider. When code is pushed to the selected branch, Envoyer will automatically trigger a new deployment.

### Delete Project

If you no longer need the project, you may delete it via the project settings dashboard. After confirming the name of the project, click the **Delete Project** button.

:::danger Deleting Projects

Deleting your project is an irreversible action and we will be unable to recover the project's settings for you.
:::
