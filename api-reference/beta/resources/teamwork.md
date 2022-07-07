---
title: teamwork 资源类型
description: 可供组织使用的 Microsoft Teams 功能的容器。
author: akjo
doc_type: resourcePageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 721335785b1fa70ad9433d1c03b7fe4c9ae89d05
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645293"
---
# <a name="teamwork-resource-type"></a>teamwork 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可供组织使用的 Microsoft Teams 功能范围的容器。

## <a name="methods"></a>方法

| 方法                                                  | 返回类型                                         |说明                                                                               |
|:--------------------------------------------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------|
|[列出 deletedTeams](../api/teamwork-list-deletedteams.md)|[deletedTeam](../resources/deletedteam.md) 集合|获取 [deletedTeam](../resources/deletedteam.md) 对象及其属性的列表。|

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|id|string| 唯一标识符。 |

## <a name="relationships"></a>关系

| 关系 | 类型 | 说明 |
|:---------------|:--------|:----------|
|deletedTeams|[deletedTeam](../resources/deletedteam.md) 集合| 已删除团队的集合。|
|设备|[teamworkDevice](../resources/teamworkdevice.md) 集合|为租户预配的 Teams 设备。|
|teamsAppSettings|[teamsAppSettings](../resources/teamsappsettings.md)|表示租户中所有 [Teams 应用](teamsapp.md) 的租户范围设置。|
|workforceIntegration|[workforceIntegration](../resources/workforceintegration.md) 集合| 工作人员与班次的集成。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamwork",
  "baseType": "microsoft.graph.entity"
}-->

``` json
{
    "@odata.type": "#microsoft.graph.teamwork",
    "id": "String (identifier)"
}
```

## <a name="see-also"></a>另请参阅

- [userTeamwork 资源类型](userteamwork.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
