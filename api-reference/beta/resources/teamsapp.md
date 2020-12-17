---
title: teamsApp 资源类型
description: Microsoft Teams 应用对话框中的应用。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: eb7c75f144f2056e610e45f86b44a19d9211f306
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706120"
---
# <a name="teamsapp-resource-type"></a>teamsApp 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表[Microsoft Teams](teams-api-overview.md) 应用目录中的一个应用.

用户可以在 Microsoft Teams 商店中看到这些应用，并且可以使用“[向团队添加应用](../api/team-post-installedapps.md)”方法将这些应用安装到 [Teams](team.md) 中。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出目录中的应用](../api/appcatalogs-list-teamsapps.md) | [teamsApp](teamsapp.md) 集合 | 列出 Microsoft Teams 应用目录中的所有应用。|
|[将应用程序上载到目录](../api/teamsapp-publish.md) | [teamsApp](teamsapp.md) | 将应用上载到组织的应用程序目录。|
|[更新目录中的应用](../api/teamsapp-update.md) | [teamsApp](teamsapp.md) | 更新组织的应用程序目录中的应用程序。|
|[从目录删除应用程序](../api/teamsapp-delete.md) | 无 | 从组织的应用程序目录中删除应用。|
|[获取与目录中的应用程序关联的机器人](../api/teamworkbot-get.md) | [teamworkbot](teamworkbot.md) | 获取与 Teams 应用关联的机器人。|

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 目录应用生成的应用 ID（不同于开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的 ID）。 |
| externalId          | string   | 应用开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的目录 ID。 |
| displayName                | string   | 应用开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的目录名称。 |
| distributionMethod  | teamsAppDistributionMethod     | 应用的分配方法。 只读。|

### <a name="teamsappdistributionmethod-values"></a>teamsAppDistributionMethod 值

|成员|值|说明|
|:---|:---|:---|
|商店|0| 应用适用于 Microsoft Teams 应用商店中的所有租户。|
|组织|1|应用仅适用于此租户。|
|旁加载|2|应用仅适用于安装它的用户/团队。|

## <a name="relationships"></a>关系

| 关系 | 类型   | 说明 |
|:---------------|:--------|:----------|
|appDefinitions|[teamsAppDefinition](teamsappdefinition.md) 集合| 每个版本的应用的详细信息。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "string",
  "distributionMethod": "string"
}
```

## <a name="see-also"></a>另请参阅

- [teamsAppInstallation](teamsappinstallation.md)
- [teamsAppDefinition](teamsappdefinition.md)
- [teamsTab](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



