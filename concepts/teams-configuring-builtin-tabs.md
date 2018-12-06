---
title: 在 Microsoft Teams 中配置内置选项卡类型
description: '使用 Microsoft Graph API 创建或配置 Microsoft Teams 选项卡 '
ms.openlocfilehash: 2485e65ebac0c7201fe8b8210f8e4af9b9c8f164
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091797"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a>在 Microsoft Teams 中配置内置选项卡类型

若要使用 Microsoft Graph API [创建](/graph/api/teamstab-add?view=graph-rest-beta)或[配置](/graph/api/teamstab-update?view=graph-rest-beta) Microsoft Teams 选项卡，你需要知道应用的 `teamsAppId` 以及为该类应用提供的 `entityId`、`contentUrl`、`removeUrl` 和 `websiteUrl`。
本文介绍如何获取内置选项卡类型的值。

## <a name="custom-tabs"></a>自定义选项卡

若要使用 Microsoft Graph 配置与所编写的[选项卡提供程序](https://docs.microsoft.com/zh-CN/microsoftteams/platform/concepts/tabs/tabs-overview)关联的选项卡，请标识 `entityId`、`contentUrl`、`removeUrl` 以及应用的[配置 UI 提供给 Microsoft Teams](https://docs.microsoft.com/zh-CN/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest) 的 `websiteUrl`，并将相同的 `entityId`、`contentUrl`、`removeUrl` 和 `websiteUrl` 值传递给 Microsoft Graph。

`teamsAppId` 与 [Microsoft Teams 的应用清单架构](https://docs.microsoft.com/zh-CN/microsoftteams/platform/resources/schema/manifest-schema)中的 `id` 相同。

## <a name="website-tabs"></a>网站选项卡

对于网站选项卡，`teamsAppId` 为 `com.microsoft.teamspace.tab.web`。 以下是配置。

| 属性   | 类型        | 说明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Null                                                     |
| contentUrl | string      | 网站的 URL                                       |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      | 网站的 URL                                       |

## <a name="planner-tabs"></a>规划器选项卡

对于规划器选项卡，teamsAppId 为 `com.microsoft.teamspace.tab.planner`。 以下是配置。

| 属性   | 类型        | 说明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | 计划 ID（要与 GET /planner/plans/{id} 一起使用的 ID）。                                              |
| contentUrl | string      | `https://tasks.office.com/{tenantName}/Home/PlannerFrame?page=7&planId={planId}`，其中 {tenantName} 是租户的名称（例如 example.onmicrosoft.com），{planId} 与实体 ID 相同。  |
| removeUrl  | string      | 与 contentUrl 的值相同。    |
| websiteUrl | string      | 与 contentUrl 的值相同。   |

若要创建在规划器选项卡中显示的新计划，请参阅[创建 plannerPlan](/graph/api/planner-post-plans?view=graph-rest-beta)。

## <a name="microsoft-stream-tabs"></a>Microsoft Stream 选项卡

对于 Microsoft Stream 选项卡，`teamsAppId` 为 `com.microsoftstream.embed.skypeteamstab`。 以下是配置。

| 属性   | 类型        | 说明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Null                                                     |
| contentUrl | string      | `https://web.microsoftstream.com/embed/video/{id}?autoplay=false&showinfo=true&app=microsoftteams&l={locale}`，其中 {id} 是视频流的 ID。 若要查找流的 {id}，请在浏览器中打开该流，然后查看 URL，它的格式应为 `https://{domain}.microsoftstream.com/video/{id}`。  |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      | `https://web.microsoftstream.com/video/{id}`，其中 {id} 是视频流的 ID。    |

## <a name="microsoft-forms-tabs"></a>Microsoft Forms 选项卡

对于 Microsoft Forms 选项卡，`teamsAppId` 为 `81fef3a6-72aa-4648-a763-de824aeafb7d`。
配置:

| 属性   | 类型        | 说明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | 表单的 ID。  定义此值，导航到 Forms 网站中的表单，然后找到表单 `https://forms.office.com/Pages/DesignPage.aspx#FormId={formId}` 的 URL。      |
| contentUrl | string      | `https://forms.office.com/Pages/TeamsDesignPage.aspx?Host=Teams&lang={locale}&groupId={groupId}&tid={tid}&teamsTheme={theme}&upn={upn}&fragment=FormId%3D{formId}`，其中 {formId} 与实体 ID 相同，{locale}、{groupId}、{tid}、{upn} 是文本。   |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      |  `https://forms.office.com`    |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a>Word、Excel、PowerPoint 和 PDF 选项卡

下表列出了每个应用的 `teamsAppId`。

| 应用   | teamsAppId | 类型（扩展名）                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| Word | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| Excel | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| PowerPoint  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| PDF | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

配置不受支持。

## <a name="wiki-tabs"></a>Wiki 选项卡

对于 wiki 选项卡，`teamsAppId` 为 `com.microsoft.teamspace.tab.wiki`。
Wiki 选项卡不支持通过 Graph 进行配置。
但请注意，不需要进行太多配置 - 在未配置的 Wiki 选项卡中，第一个用户只需单击“设置选项卡”**** 即可对其进行配置。

## <a name="document-library-tabs"></a>文档库选项卡

对于文档库选项卡，`teamsAppId` 为 `com.microsoft.teamspace.tab.files.sharepoint`。 配置不受支持。

## <a name="onenote-tabs"></a>OneNote 选项卡

对于 OneNote 选项卡，`teamsAppId` 为 `0d820ecd-def2-4297-adad-78056cde7c78`。 以下是配置。

| 属性   | 类型        | 说明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | `{randomGuid}_{notebookId}`，其中 {randomGuid} 是所生成的 GUID。                                      |
| contentUrl | string      | 表单 `https://www.onenote.com/teams/TabContent?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{sectionsUrl}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}` 的 URL，其中 `{sectionsUrl}`、`{notebookId}` 和 `{oneNoteWebUrl}` 均可在 [GET /groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta) 中找到。 斜杠必须经过转义。 {locale} 和 {tid} 是文本。 |
| removeUrl  | string      | 表单 `https://www.onenote.com/teams/TabRemove?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{sectionsUrl}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}` 的 URL，其中 `{sectionsUrl}`、`{notebookId}` 和 `{oneNoteWebUrl}` 均可在 [GET /groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta) 中找到。 斜杠必须经过转义。 {locale} 和 {tid} 是文本。 |
| websiteUrl | string      | 表单 `https://www.onenote.com/teams/TabRedirect?redirectUrl={oneNoteWebUrl}` 的 URL，其中 `oneNoteWebUrl` 可以在 [GET /groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta) 中找到 |

## <a name="power-bi-tabs"></a>Power BI 选项卡

对于 Power BI 选项卡，`teamsAppId` 为 `com.microsoft.teamspace.tab.powerbi`。
配置不受支持。

## <a name="sharepoint-page-and-list-tabs"></a>SharePoint 页和列表选项卡

对于 SharePoint 页和列表选项卡，`teamsAppId` 为 `2a527703-1f6f-4559-a332-d8a7d288cd88`。
配置不受支持。
如果需要配置，请考虑使用网站选项卡。
