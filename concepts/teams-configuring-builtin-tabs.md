---
title: 在 Microsoft 团队中配置的内置选项卡类型
description: '若要创建或配置使用 Microsoft Graph Api 的 Microsoft 团队选项卡 '
ms.openlocfilehash: 2485e65ebac0c7201fe8b8210f8e4af9b9c8f164
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091797"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a>在 Microsoft 团队中配置的内置选项卡类型

[创建](/graph/api/teamstab-add?view=graph-rest-beta)或[配置](/graph/api/teamstab-update?view=graph-rest-beta)使用 Microsoft Graph Api 的 Microsoft 团队选项卡，您需要知道`teamsAppId`的应用程序和`entityId`， `contentUrl`， `removeUrl`，和`websiteUrl`提供该类型的应用程序。
本文说明如何获取这些值的内置选项卡的类型。

## <a name="custom-tabs"></a>自定义选项卡

若要使用 Microsoft Graph 配置编写[选项卡提供程序](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview)相关联的一个选项卡，确定`entityId`， `contentUrl`， `removeUrl`，和`websiteUrl`的应用程序的[UI 提供的 Microsoft 团队的配置](https://docs.microsoft.com/en-us/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest)，并传递相同`entityId`， `contentUrl`， `removeUrl`，和`websiteUrl`值到 Microsoft Graph。

`teamsAppId`相同`id`在[应用程序清单架构的 Microsoft 团队](https://docs.microsoft.com/en-us/microsoftteams/platform/resources/schema/manifest-schema)。

## <a name="website-tabs"></a>网站选项卡

对于网站选项卡，`teamsAppId`是`com.microsoft.teamspace.tab.web`。 下面是配置。

| 属性   | 类型        | 说明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Null                                                     |
| contentUrl | string      | 网站的 URL                                       |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      | 网站的 URL                                       |

## <a name="planner-tabs"></a>计划工具选项卡

对于计划工具选项卡，teamsAppId 是`com.microsoft.teamspace.tab.planner`。 下面是配置。

| 属性   | 类型        | 说明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | 计划 ID (使用 GET /planner/计划 / {id} ID) 中。                                              |
| contentUrl | string      | `https://tasks.office.com/{tenantName}/Home/PlannerFrame?page=7&planId={planId}`其中 {tenantName} 是 （如 example.onmicrosoft.com)，租户的名称，{planId} 是与实体 ID 相同。  |
| removeUrl  | string      | ContentUrl 相同的值。    |
| websiteUrl | string      | ContentUrl 相同的值。   |

若要创建新的计划以在您计划工具选项卡中显示，请参阅[创建 plannerPlan](/graph/api/planner-post-plans?view=graph-rest-beta)。

## <a name="microsoft-stream-tabs"></a>Microsoft 流选项卡

对于 Microsoft 流选项卡，`teamsAppId`是`com.microsoftstream.embed.skypeteamstab`。 下面是配置。

| 属性   | 类型        | 说明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Null                                                     |
| contentUrl | string      | `https://web.microsoftstream.com/embed/video/{id}?autoplay=false&showinfo=true&app=microsoftteams&l={locale}`其中 {id} 是视频流的 ID。 若要查找流 {id}，在浏览器中打开流和一下您 URL – 将窗体的`https://{domain}.microsoftstream.com/video/{id}`。  |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      | `https://web.microsoftstream.com/video/{id}`其中 {id} 是视频流的 ID。    |

## <a name="microsoft-forms-tabs"></a>Microsoft Forms 选项卡

对于 Microsoft Forms 选项卡，`teamsAppId`是`81fef3a6-72aa-4648-a763-de824aeafb7d`。
配置：

| 属性   | 类型        | 说明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | 表单的 ID。  定义此值，导航到窗体网站中的窗体并查找表单的 URL `https://forms.office.com/Pages/DesignPage.aspx#FormId={formId}`。      |
| contentUrl | string      | `https://forms.office.com/Pages/TeamsDesignPage.aspx?Host=Teams&lang={locale}&groupId={groupId}&tid={tid}&teamsTheme={theme}&upn={upn}&fragment=FormId%3D{formId}`其中 {formId} 是相同的实体 ID 和 {区域设置}，为 {groupId} {tid} {upn} 是文字。   |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      |  `https://forms.office.com`    |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a>Word、 Excel、 PowerPoint 和 PDF 选项卡

下表列出`teamsAppId`每个应用程序。

| App   | teamsAppId | 类型 （扩展）                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| Word | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| Excel | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| PowerPoint  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| PDF | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

不支持配置。

## <a name="wiki-tabs"></a>Wiki 选项卡

对于 wiki 选项卡，`teamsAppId`是`com.microsoft.teamspace.tab.wiki`。
Wiki 选项卡不支持通过图形的配置。
但请注意，没有何配置-中未配置 wiki 选项卡上，第一个用户只需要单击**设置选项卡上**来配置它。

## <a name="document-library-tabs"></a>文档库选项卡

对于文档库选项卡中，`teamsAppId`是`com.microsoft.teamspace.tab.files.sharepoint`。 不支持配置。

## <a name="onenote-tabs"></a>OneNote 选项卡

对于 OneNote 选项卡，`teamsAppId`是`0d820ecd-def2-4297-adad-78056cde7c78`。 下面是配置。

| 属性   | 类型        | 说明                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | `{randomGuid}_{notebookId}`其中 {randomGuid} 是，生成的 GUID。                                      |
| contentUrl | string      | 表单的 URL `https://www.onenote.com/teams/TabContent?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{sectionsUrl}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}`，其中`{sectionsUrl}`， `{notebookId}`，和`{oneNoteWebUrl}`可以在[获取 /groups/ {id} / onenote/笔记本](/graph/api/onenote-list-notebooks?view=graph-rest-beta)中找到。 斜杠必须对它们进行转义。 {区域设置} 和 {tid} 是文字。 |
| removeUrl  | string      | 表单的 URL `https://www.onenote.com/teams/TabRemove?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{sectionsUrl}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}`，其中`{sectionsUrl}`， `{notebookId}`，和`{oneNoteWebUrl}`可以在[获取 /groups/ {id} / onenote/笔记本](/graph/api/onenote-list-notebooks?view=graph-rest-beta)中找到。 斜杠必须对它们进行转义。 {区域设置} 和 {tid} 是文字。 |
| websiteUrl | string      | 表单的 URL `https://www.onenote.com/teams/TabRedirect?redirectUrl={oneNoteWebUrl}`，其中`oneNoteWebUrl`可以找到中[获取 /groups/ {id} / onenote/笔记本](/graph/api/onenote-list-notebooks?view=graph-rest-beta) |

## <a name="power-bi-tabs"></a>Power BI 选项卡

Power BI 选项卡，`teamsAppId`是`com.microsoft.teamspace.tab.powerbi`。
不支持配置。

## <a name="sharepoint-page-and-list-tabs"></a>SharePoint 页面和列表选项卡

对于 SharePoint 页面和列表选项卡，`teamsAppId`是`2a527703-1f6f-4559-a332-d8a7d288cd88`。
不支持配置。
如果需要配置，请考虑使用网站选项卡。
