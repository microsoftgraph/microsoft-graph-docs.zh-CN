---
title: 团队资源类型
description: 'Microsoft Teams 团队是频道的集合。 '
author: AkJo
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 554e16245616605a86beb797adfca0370e948e49
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519675"
---
# <a name="team-resource-type"></a>团队资源类型

命名空间：microsoft.graph



Microsoft Teams 中的团队是 [channel](channel.md) 对象的集合。
频道表示团队内部的某个主题，因此是讨论的逻辑隔离。

每个团队与一个[组](../resources/group.md)相关联。
该组具有与团队相同的 ID，例如 `/groups/{id}/team` 与 `/teams/{id}` 相同。
有关使用组和团队内部成员的详细信息，请参阅[使用 Microsoft Graph REST API 来处理 Microsoft Teams](teams-api-overview.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建团队](../api/team-post.md) | [teamsAsyncOperation](teamsasyncoperation.md) | 从头开始创建团队。 |
|[从组创建团队](../api/team-put-teams.md) | [team](team.md) | 创建新的团队，或向现有组添加团队。|
|[获取团队](../api/team-get.md) | [team](team.md) | 检索指定团队的属性和关系。|
|[更新团队](../api/team-update.md) | [team](team.md) |更新指定团队的属性。 |
|[删除团队](../api/group-delete.md) | 无 |删除团队及其关联的组。 |
|[List members](../api/team-list-members.md)|[conversationMember](../resources/conversationmember.md) 集合|获取此团队中的成员列表。|
|[添加成员](../api/team-post-members.md)|[conversationMember](../resources/conversationmember.md)|向团队中添加新成员。|
|[批量添加成员](../api/conversationmembers-add.md)|[actionResultPart](../resources/actionresultpart.md) 集合|在单个请求中将多个成员添加到团队中。|
|[获取成员](../api/team-get-members.md) | [conversationMember](conversationmember.md) 集合 | 获取团队中的成员。|
|[更新成员角色](../api/team-update-members.md)|[conversationMember](../resources/conversationmember.md)|将成员更改为所有者或返回为常规成员。|
|[删除成员](../api/team-delete-members.md)|无|删除团队中的一个现有成员。|
|[存档团队](../api/team-archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |将团队置于只读状态。 |
|[解档团队](../api/team-unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |将团队还原到读写状态。 |
|[克隆团队](../api/team-clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |复制团队及其关联的组。 |
|[列出你的团队](../api/user-list-joinedteams.md) | [team](team.md) 集合 | 列出你属于的团队。 |
|[完成迁移](../api/team-completemigration.md)|[团队](team.md)| 从团队中删除迁移模式并使团队可供用户发布和阅读消息。|
|[列出团队中安装的应用](../api/team-list-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) 集合 | 列出团队中安装的应用。|
|[将应用添加到团队](../api/team-post-installedapps.md) |无 | 向团队添加（安装）应用程序。|
|[获取团队中安装的应用](../api/team-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | 获取团队中安装的指定应用。|
|[升级团队中安装的应用](../api/team-teamsappinstallation-upgrade.md) | 无 | 将团队中安装的应用程序升级到最新版本。|
|[从团队中删除应用](../api/team-delete-installedapps.md) | 无 | 从团队中删除（卸载）应用。|

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|displayName|string| 团队的名称。 |
|description|string| 组的说明（可选）。 最大长度：1024 个字符。 |
|classification|string| 标签（可选）。 通常说明团队的数据或业务敏感性。 必须与租户目录中的一个预配置集匹配。 |
|specialization|[teamSpecialization](teamspecialization.md)| 可选。 指示团队是否适用于特定用例。  每个团队专用化都可以访问针对其用例的独特行为和体验。 |
|visibility|[teamVisibilityType](teamvisibilitytype.md)| 组和团队的可见性。默认值为 Public。 |
|funSettings|[teamFunSettings](teamfunsettings.md) |用于配置团队中 Giphy、成员和贴纸使用情况的设置。|
|guestSettings|[teamGuestSettings](teamguestsettings.md) |用于配置来宾是否可以在团队中创建、更新或删除频道的设置。|
|internalId | 字符串 | 已在一些位置（如审核日志/[Office 365 管理活动 API](/office/office-365-management-api/office-365-management-activity-api-reference)）使用的团队唯一 ID。 |
|isArchived|Boolean|此团队是否处于只读模式。 |
|memberSettings|[teamMemberSettings](teammembersettings.md) |用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。|
|messagingSettings|[teamMessagingSettings](teammessagingsettings.md) |用于配置团队中的消息传递和提及的设置。|
|webUrl|string (readonly) | 用于转到 Microsoft Teams 客户端中团队的超链接。 这是在 Microsoft Teams 客户端中右键单击团队并选择 **获取团队链接** 时获取的 URL。 应将此 URL 视为不透明的 blob，而不对其进行解析。 |
|createdDateTime|dateTimeOffset|创建团队的时间戳。|

### <a name="instance-attributes"></a>实例属性

实例属性是具有特殊行为的属性。这些属性是临时的，并且 a) 定义服务应执行的行为或 b) 提供短期的属性值，例如过期项目的下载 URL。

| 属性名称| 类型   | 说明
|:-----------------------|:-------|:-------------------------|
|@microsoft. graph teamCreationMode|string|指示团队处于迁移状态，并且当前正用于迁移目的。 它接受一个值：`migration`。 **注意**：将来，Microsoft 可能会要求你或你的客户根据导入的数据量支付其他费用。|

有关 POST 请求示例，请参阅[请求（创建处于迁移状态的团队）](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)。

## <a name="relationships"></a>关系

| 关系 | 类型 | 说明 |
|:---------------|:--------|:----------|
|channels|[channel](channel.md) 集合|与团队相关的频道和消息的集合。|
|installedApps|[teamsAppInstallation](teamsappinstallation.md) 集合|此团队中安装的应用。|
|members|[conversationMember](../resources/conversationmember.md) 集合|团队的成员和所有者。|
|operations|[teamsAsyncOperation](teamsasyncoperation.md) 集合| 在此团队中运行过或正在运行的异步操作。 | 
|[primaryChannel](../api/team-get-primarychannel.md)|[频道](channel.md)| 团队的常规频道。 | 
|schedule|[日程安排](schedule.md)| 此团队的排班安排。|
|template|[teamsTemplate](teamstemplate.md)| 创建此团队时所使用的模板。 请参阅[可用模板](/MicrosoftTeams/get-started-with-teams-templates)。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

>**注意：** 如果团队属于班级类型，则会在团队上应用 **classSettings** 属性。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.team",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "guestSettings": {"@odata.type": "microsoft.graph.teamGuestSettings"},
  "memberSettings": {"@odata.type": "microsoft.graph.teamMemberSettings"},
  "messagingSettings": {"@odata.type": "microsoft.graph.teamMessagingSettings"},
  "funSettings": {"@odata.type": "microsoft.graph.teamFunSettings"},
  "internalId": "string",
  "isArchived": false,
  "webUrl": "string (URL)",
  "classSettings": {"@odata.type": "microsoft.graph.teamClassSettings"},
  "createdDateTime": "dateTimeOffset"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a>另请参阅

- [将 Microsoft Graph API 与 Microsoft Teams 结合使用](teams-api-overview.md)
- [创建包含团队的组](/graph/teams-create-group-and-team)
- [列出所有团队](/graph/teams-list-all-teams)

