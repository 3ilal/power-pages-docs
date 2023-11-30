﻿---
title: "How to: replace the default Power Pages AI chatbot with a Power Virtual Agents bot"
description: Learn how to replace the default Power Pages AI chatbot with a Power Virtual Agents bot.
ms.topic: how-to
ms.date: 11/30/2023
author: nageshbhat-msft
ms.author: nabha
ms.reviewer: kkendrick
contributors:
  - ProfessorKendrick
  - nageshbhat-msft
ms.custom: bap-template
---

# How to: replace the default Power Pages AI chatbot with a Power Virtual Agents bot

This article offers a comprehensive, step-by-step guide for updating default Power Pages AI chatbot with Power Virtual Agents bot.

## Prerequisite

-  You must have a bot created in [Power Virtual Agent](/power-virtual-agents/nlu-gpt-quickstart#create-a-boosted-bot).

-  Your [AI chatbot](enable-chatbot.md#add-a-chatbot) must be created and published in the site where you're updating the Power Virtual Agents bot.

## Copy the bot schema name

1. Sign in to [Power Virtual Agents](https://web.powerva.microsoft.com/).

1. Select the bot, which needs to be updated.

1. Navigate to **Copilot details** under **Settings**.

1. Select **Advanced** tab.

1. Copy the **Schema name**.

## Verify Data model version

AI chatbot can be enabled for both Standard and Enhanced site data model. The steps to replace it vary based on the data model. Make sure you're following the right steps based on the data model.

1. Go to the [Set up workspace](../configure/setup-workspace.md).

1. Select **Site details**.

1. Verify the **Data Model** version. You can choose **Standard** or **Enhanced**.

## Update the bot in Standard data model site

1. Go to the [Data workspace](use-data-workspace.md).

1. Search for and select the **Bot consumer** table.

1. Locate the row with selected website name.

1. Replace the Bot Schema Name column value with new bot schema name you copied earlier.

## Update the bot in Enhanced data model

1. Go to the [Data workspace](use-data-workspace.md).

1. Search for and select the **Site Component** table.

1. Find the **Component Type** column and select the filter icon next to it.

1. Filter records by **Bot Consumer** option.

1. Locate the row with selected website name in the **Power Pages Site id** column.

1. Choose **Edit row using form**.

1. Replace **botschemaname** json value with the new bot schema name you copied earlier.

1. Choose **Save & Close**.
