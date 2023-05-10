---
title: Customize webpages with design studio page editor
description: Learn how to customize Power Pages sites with the design studio page editor.
author: clromano
ms.topic: conceptual
ms.custom: 
ms.date: 05/09/2023
ms.subservice:
ms.author: clromano 
ms.reviewer: kkendrick
contributors:
    - clromano
    - nickdoelman
    - ProfessorKendrick
---

# Customize webpages with design studio page editor

After adding the webpages you need and managing their hierarchy in the site map, you can add various components. The WYSIWYG design studio page editor is part of the Pages workspace. Use the editor to add and edit the components you need within the canvas.

### Using the editor

To use the editor:

1. Open the [design studio](use-design-studio.md) to edit the content and components of the portal.

1. Go to the **Pages** workspace.

1. Select the page where you'd like to add the component or section.

1. To add a section, hover over any editable section area, and then select the plus sign (**+**). You can then choose between six section layout options.

    :::image type="content" source="media/common/add-section-layout.png" alt-text="The six section layout options.":::

1. To add a component, hover over the section where you'd like to place the component, and then select **+**. You can then choose between the available components.  

    :::image type="content" source="media/common/component-options.png" alt-text="The add component menu options.":::
    
    You can drag and drop sections, columns, and components to re-arrange them on a page.

    To drag an object, left-click and hold down the mouse button, or press the space bar while it's focused. Next, drag the object to the target area using the mouse or keyboard arrows. Drop zones will appear to indicate where the object can be placed. Once you reach the drop zone, release the left mouse button or press the space bar to drop the object.
    
    >[!NOTE]
    > - Some components are not draggable, including the header, footer, and some nested components (links within a text component, for example). 
    > - Drag and drop functionality is not supported for sections that have the ```flex-direction``` CSS property set to ```row-reverse```.

1. To delete a component, choose the component on the canvas and then select **Delete**.

For a more immersive editing experience, you can use the full-screen editing mode by selecting the double arrow icon in the upper-right corner of the editor. You can also switch to [Visual Studio Code](../configure/visual-studio-code-editor.md), **zoom in (+)**,  **zoom out (-)**, or **Reset** the page design canvas view back to 100%.

:::image type="content" source="media/common/page-edit-options.png" alt-text="Controls for immersive editing options, including zoom in, zoom out, and reset.":::

All sections and components allow for in-context editing. You can edit any section or component directly from the canvas.

Select the paintbrush icon to adjust the styles of a section or component. Different styles are available based on the component's type. Currently, sections, text, images, and video are supported.

## Undo/Redo (preview)

[!INCLUDE [cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]


In the Pages workspace, you'll see undo/redo buttons in the top left of the canvas. The undo button is enabled when you make a change. The redo button is enabled when you undo an action.

:::image type="content" source="media/common/undo-redo.png" alt-text="The Pages workspace with the undo/redo buttons displayed.":::

To reverse an action, select the Undo button.

To reverse an undo, select the Redo button.

Undo and redo only support changes that you make in the Pages workspace.  Your action history clears when you refresh the browser page or navigate to another workspace inside the design studio.

### Limitations

Syncing, saving, previewing, zooming , expanding/reducing the workspace, navigating between workspaces and pages, and uploading media and CSS files are not supported.

> [!NOTE]
> - You cannot delete the header or footer in the Pages workspace. See [Web templates](../configure/web-templates.md) for information on creating custom page layouts.
> - For sites created using Power Pages prior to September 23, 2022 there is a known issue related to themes. More information: [Adjusting the background color for your Power Pages site](../known-issues.md#adjusting-the-background-color-for-your-power-pages-site)

### See also

- [Add text](add-text.md)
- [Add button](add-button.md)
- [Add image](add-image.md)
- [Add video](add-video.md)
- [Add spacer](add-spacer.md)
- [Add Power BI](add-power-bi.md)
- [Add list](add-list.md)
- [Add form](add-form.md)
- [Add IFrame](add-iframe.md)
- [Add multistep form](multistep-forms.md)
- [Edit code with Visual Studio Code for the Web](../configure/visual-studio-code-editor.md)
- [Structure site map](structure-site.md)
