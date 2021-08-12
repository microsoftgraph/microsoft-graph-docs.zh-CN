---
title: 在 Microsoft Teams 中配置内置选项卡类型
description: 使用 Microsoft Graph API 创建或配置 Microsoft Teams 选项卡
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2decc60c3315ef6f324d35afce2ff10617c85e716ec7282215053c478ef729b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54225718"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a>在 Microsoft Teams 中配置内置选项卡类型

若要使用 Microsoft Graph API [创建](/graph/api/channel-post-tabs?view=graph-rest-1.0)或[配置](/graph/api/channel-patch-tabs?view=graph-rest-1.0) Microsoft Teams 选项卡，你需要知道应用的 `teamsAppId` 以及为该类应用提供的 `entityId`、`contentUrl`、`removeUrl` 和 `websiteUrl`。
本文介绍如何获取内置选项卡类型的值。

## <a name="custom-tabs"></a>自定义选项卡

若要使用 Microsoft Graph 配置与所编写的[选项卡提供程序](/microsoftteams/platform/concepts/tabs/tabs-overview)关联的选项卡，请标识 `entityId`、`contentUrl`、`removeUrl` 以及应用的[配置 UI 提供给 Microsoft Teams](/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest) 的 `websiteUrl`，并将相同的 `entityId`、`contentUrl`、`removeUrl` 和 `websiteUrl` 值传递给 Microsoft Graph。

`teamsAppId` 与 [Microsoft Teams 的应用清单架构](/microsoftteams/platform/resources/schema/manifest-schema)中的 `id` 相同。

## <a name="website-tabs"></a>网站选项卡

对于网站选项卡，`teamsAppId` 为 `com.microsoft.teamspace.tab.web`。 以下是配置。

| 属性   | 类型        | 说明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Null                                                     |
| contentUrl | string      | 网站的 URL                                       |
| removeUrl  | string      | Null                                                     |
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
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      | Null                                       |

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

## <a name="document-library-tabs"></a>文档库选项卡

对于文档库选项卡，`teamsAppId` 为 `com.microsoft.teamspace.tab.files.sharepoint`。 以下是配置。

| 属性   | 类型        | 说明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | 空字符串 ("")                                         |
| contentUrl | string      | 文档库的根文件夹的 URL。 可以通过在浏览器中打开 SharePoint 文件夹、复制 URL 并删除"/Forms/AllItems.aspx"以及之后的所有内容来查找此 URL。 |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      | Null                                                     |

### <a name="example-create-a-configured-document-library-tab"></a>示例：创建配置的文档库选项卡

下面的示例创建一个配置的文档库选项卡。

```http
POST https://graph.microsoft.com/v1.0/teams/{team-id}/channels/{channel-id}/tabs
{
    "displayName": "Document%20Library1",
    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/com.microsoft.teamspace.tab.files.sharepoint",
    "configuration": {
        "entityId": "",
        "contentUrl": "https://microsoft.sharepoint.com/teams/WWWtest/Shared%20Documents",
        "removeUrl": null,
        "websiteUrl": null
    }
}
```

## <a name="wiki-tabs"></a>Wiki 选项卡

对于 wiki 选项卡，`teamsAppId` 为 `com.microsoft.teamspace.tab.wiki`。
Wiki 选项卡不支持通过 Microsoft Graph。
但是请注意，没有太多要配置的内容 -在未配置的 Wiki 选项卡中，第一个用户只需选择" **设置** "选项卡来配置它。

## <a name="planner-tabs"></a>Planner 选项卡

对于 Planner 选项卡， `teamsAppId` 为 `com.microsoft.teamspace.tab.planner` 。 配置不受支持。

## <a name="microsoft-stream-tabs"></a>Microsoft Stream 选项卡

对于 Microsoft Stream 选项卡，`teamsAppId` 为 `com.microsoftstream.embed.skypeteamstab`。 配置不受支持。

## <a name="microsoft-forms-tabs"></a>Microsoft Forms 选项卡

对于 Microsoft Forms 选项卡，`teamsAppId` 为 `81fef3a6-72aa-4648-a763-de824aeafb7d`。
配置不受支持。

## <a name="onenote-tabs"></a>OneNote 选项卡

对于 OneNote 选项卡，`teamsAppId` 为 `0d820ecd-def2-4297-adad-78056cde7c78`。 配置不受支持。

## <a name="power-bi-tabs"></a>Power BI 选项卡

对于 Power BI 选项卡，`teamsAppId` 为 `com.microsoft.teamspace.tab.powerbi`。
配置不受支持。

## <a name="sharepoint-page-and-list-tabs"></a>SharePoint 页和列表选项卡

对于 SharePoint 页和列表选项卡，`teamsAppId` 为 `2a527703-1f6f-4559-a332-d8a7d288cd88`。
配置不受支持。
若你想要配置选项卡，请考虑使用网站选项卡。
