---
title: Use code components in Power Pages
description: Learn about creating code components for model-driven and canvas apps using Power Apps component framework inside Power Pages.
author: GitanjaliSingh33msft

ms.topic: conceptual
ms.custom: 
ms.date: 01/31/2023
ms.subservice: 
ms.author: gisingh
ms.reviewer: ndoelman
contributors:
  - nickdoelman
  - GitanjaliSingh33msft
  - HemantGaur
  - ProfessorKendrick
---

# Use code components in Power Pages

Power Apps component framework empowers professional developers and app makers to create code components for model-driven and canvas apps. These code components can provide an enhanced experience for users working with data on forms, views, and dashboards. More information: [Power Apps component framework overview](/power-apps/developer/component-framework/overview.md)

Power Pages now supports controls built for model-driven apps created using Power Apps component framework. To use code components in Power Pages site webpages, follow these steps:

:::image type="content" source="media/component-framework/steps.png" alt-text="Create code component using component framework, then add the code component to a model-driven app form, and configure the code component field inside the basic form for portals.":::

After following these steps, your users can now interact with the code component using the webpage that has the respective [form](../getting-started/add-form.md) component.  

## Prerequisites

- You must have System Administrator privileges to enable the code component feature in the environment.
- Your Power Pages site version must be [9.3.3.x](/power-apps/maker/portals/versions/version-9.3.3.x) or higher.
- Your starter site package must be [9.2.2103.x](/power-apps/maker/portals/versions/package-version-9.2.2103) or higher.

## Create and package code component

To learn about creating and packaging code components created Power Apps component framework, go to [Create your first component](/power-apps/developer/component-framework/implementing-controls-using-typescript).

### Supported field types and formats

Power Pages supports restricted field types and formats for using code components. The following table lists all supported field data types and formats:

:::row:::
   :::column span="":::
      Currency
   :::column-end:::
   :::column span="":::
      DateAndTime.DateAndTime
   :::column-end:::
   :::column span="":::
      DateAndTime.DateOnly
   :::column-end:::
   :::column span="":::
      Decimal
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="":::
      Enum
   :::column-end:::
   :::column span="":::
      Floating Point Number
   :::column-end:::
   :::column span="":::
      Multiple
   :::column-end:::
   :::column span="":::
      OptionSet
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="":::
      SingleLine.Email
   :::column-end:::
   :::column span="":::
      SingleLine.Phone
   :::column-end:::
   :::column span="":::
      SingleLine.Text
   :::column-end:::
   :::column span="":::
      SingleLine.TextArea
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="":::
      SingleLine.Ticker
   :::column-end:::
   :::column span="":::
      SingleLine.URL
   :::column-end:::
   :::column span="":::
      TwoOptions
   :::column-end:::
   :::column span="":::
      Whole
   :::column-end:::
:::row-end:::

More information: [Attributes list and descriptions](/power-apps/developer/component-framework/manifest-schema-reference/property#remarks)

### Unsupported code components in Power Pages

-   The following code component APIs aren’t supported:

    -   [Device.captureAudio](/power-apps/developer/component-framework/reference/device/captureaudio.md)

    -   [Device.captureImage](/power-apps/developer/component-framework/reference/device/captureimage.md)

    -   [Device.captureVideo](/power-apps/developer/component-framework/reference/device/capturevideo.md)

    -   [Device.getBarcodeValue](/power-apps/developer/component-framework/reference/device/getbarcodevalue.md)

    -   [Device.getCurrentPosition](/power-apps/developer/component-framework/reference/device/getcurrentposition.md)

    -   [Device.pickFile](/power-apps/developer/component-framework/reference/device/pickfile.md)

    -   [Utility](/power-apps/developer/component-framework/reference/utility.md)

-   The [uses-feature](/power-apps/developer/component-framework/manifest-schema-reference/uses-feature.md) element must not be set to **true**.

-   [Value elements not supported](/power-apps/developer/component-framework/manifest-schema-reference/property.md#value-elements-that-are-not-supported)
    by Power Apps component framework.

## Add a code component to a field in a model-driven app

To learn how to add a code component to a field in model-driven app, go to [Add a code component to a field](/power-apps/developer/component-framework/add-custom-controls-to-a-field-or-entity#add-a-code-component-to-a-column).

> [!IMPORTANT]
> Code components for Power Pages are available for web browsers using the client option of **Web**.

## Configure Power Pages site for code component

After the code component is added to a field in a model-driven app, you can configure Power Pages to use the code component on a form.

There are two methods to enable the code component.

### Enable code component in design studio

Open the Power Pages design studio

### Enable code component in Portals Management app

To add a code component to a basic form using the Portal Management app:

1. Open the [Portals Management](portal-management-app.md) app.

1. On the left pane, select **Basic Forms**.

1. Select the form to which you want to add the code component.

1. Select **Related**.

1. Select **Basic Form Metadata**.

1. Select **New Basic Form Metadata**.

1. Select **Type** as **Attribute**.

1. Select **Attribute Logical Name.**

1. Enter **Label**.

1. For **Control Style**, select **Code Component.**

1. Save and close the form.

## Code components using the portal Web API

A code component can be built and added to a webpage that can use the [portal Web API](web-api-overview.md) to perform create, retrieve, update, and delete actions. This feature allows greater customization options when developing portal solutions. For more information, go to [Implement a sample portal Web API component](implement-webapi-component.md).

## Next steps

[Tutorial: Use code components in portals](component-framework-tutorial.md)

### See also

- [Power Apps component framework overview](/power-apps/developer/component-framework/overview) 
- [Create your first component](/power-apps/developer/component-framework/implementing-controls-using-typescript) 
- [Add code components to a column or table in model-driven apps](/power-apps/developer/component-framework/add-custom-controls-to-a-field-or-entity)


