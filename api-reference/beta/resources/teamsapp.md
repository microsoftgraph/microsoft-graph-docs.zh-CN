---
title: teamsApp 资源类型
description: Microsoft 团队应用程序目录中的应用程序。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe60222ae6c5d8475722e18e69555df2d3892759
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553948"
---
# <a name="teamsapp-resource-type"></a>teamsApp 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Microsoft 团队](teams-api-overview.md)应用程序目录中的应用程序。

用户可以在 Microsoft 团队存储中查看这些应用程序, 并且可以使用 "向[团队添加应用程序](../api/teamsappinstallation-add.md)" 方法在[团队](team.md)中安装这些应用程序。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出已发布的应用程序](../api/teamsapp-list.md) | [teamsApp](teamsapp.md) 集合 | 列出 Microsoft 团队应用程序目录中的已发布应用程序。|
|[发布应用程序](../api/teamsapp-publish.md) | [teamsApp](teamsapp.md) | 将应用程序发布到组织的应用程序目录。|
|[更新已发布的应用程序](../api/teamsapp-update.md) | [teamsApp](teamsapp.md) | 更新组织的应用程序目录中的已发布应用程序。|
|[删除已发布的应用程序](../api/teamsapp-delete.md) | 无 | 从组织的应用程序目录中删除已发布的应用程序。|

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 目录应用程序生成的应用程序 id (与[Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中开发人员提供的 id 不同。 |
| externalId          | string   | [Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中的应用程序开发人员提供的目录的 ID。 |
| displayName                | string   | [Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中的应用程序开发人员提供的目录应用程序的名称。 |
| distributionMethod  | teamsAppDistributionMethod     | 应用的分发方法。 |

### <a name="teamsappdistributionmethod-values"></a>teamsAppDistributionMethod 值

|Member|值|说明|
|:---|:---|:---|
|microsoft|0| 该应用程序可通过 Microsoft 团队应用商店对所有租户可用。|
|组织|1|该应用程序仅在此租户中可用。|
|旁加载|2 |该应用程序仅适用于其安装到的用户/团队。|

## <a name="relationships"></a>关系

| 关系 | 类型   | 说明 |
|:---------------|:--------|:----------|
|appDefinitions|[teamsAppDefinition](teamsappdefinition.md)集合| 每个版本的应用程序的详细信息。 |

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
  "displayName": "Test App",
  "distributionMethod": "Organization"
}
```

# <a name="see-also"></a>另请参阅

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
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsapp.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

