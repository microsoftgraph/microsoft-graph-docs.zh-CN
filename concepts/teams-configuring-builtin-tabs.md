---
title: 在 Microsoft Teams 中配置内置选项卡类型
description: 使用 Microsoft Graph API 创建或配置 Microsoft Teams 选项卡
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ffe2799f557b12dd72fa72e6bf8b20f72f507647
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345987"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a>在 Microsoft Teams 中配置内置选项卡类型

若要使用 Microsoft Graph API [创建](/graph/api/teamstab-add?view=graph-rest-beta)或[配置](/graph/api/teamstab-update?view=graph-rest-beta) Microsoft Teams 选项卡，你需要知道应用的 `teamsAppId` 以及为该类应用提供的 `entityId`、`contentUrl`、`removeUrl` 和 `websiteUrl`。
本文介绍如何获取内置选项卡类型的值。

## <a name="website-tabs"></a>网站选项卡

对于网站选项卡，`teamsAppId` 为 `com.microsoft.teamspace.tab.web`。 以下是配置。

| 属性   | 类型        | 说明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | 字符串      | Null                                                     |
| contentUrl | string      | 网站的 URL                                       |
| removeUrl  | 字符串      | Null                                                     |
| websiteUrl | string      | 网站的 URL                                       |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a>Word、Excel、PowerPoint 和 PDF 选项卡

下表列出了每个应用的 `teamsAppId`。

| 应用   | teamsAppId | 类型（扩展名）                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| Word | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| Excel | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| PowerPoint  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| PDF | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

以下是配置。

| 属性   | 类型        | 说明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | 字符串      | 文件的 sourceDoc ID。 通过打开 SharePoint 中文件并查看地址栏即可找到 – URL 将有一个`sourcedoc=%7B{sourceDocId}%7D`子句。 此外还可从文档 SharePoint 驱动器项的 webUrl 派生。 有关详细信息，请参阅 [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta)。 |
| contentUrl | 字符串      | `{folder-webUrl}/{item-name}` 格式文件的 URL。 {folder-webUrl} 是包含文件的 SharePoint 文件夹 webUrl，通过打开 SharePoint 中文件并查看地址栏，或使用 [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta) 的 webUrl 属性即可找到该文件。 {item-name} 是文件名（例如 file.docx），也就是 [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta) 中的 `name` 属性。 |
| removeUrl  | 字符串      | Null                                                     |
| websiteUrl | 字符串      | Null                                       |

### <a name="example-create-a-configured-word-tab"></a>示例： 创建一个配置好的 Word 选项卡

以下示例将新建一个配置好的 Word 选项卡。

```http
POST https://graph.microsoft.com/v1.0/teams/{team-id}/channels/{channel-id}/tabs
{
  "displayName": "word",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/com.microsoft.teamspace.tab.file.staticviewer.word",
  "configuration": {
     "entityId": "115A90F4-AC9C-4F79-9837-36D1EFB3BE08",
     "contentUrl": "https://m365x165177.sharepoint.com/sites/4NewCloneWithClonableParts/Shared%20Documents/General/Employee Handbook.docx",
     "removeUrl": null,
     "websiteUrl": null
  }
}
```
