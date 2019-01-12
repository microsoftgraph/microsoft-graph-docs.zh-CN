---
title: teamsAppInstallation 资源类型
description: '团队中安装 teamsApp。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 153b131cd24709995d7215b1cf568a8565f42a80
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929478"
---
# <a name="teamsappinstallation-resource-type"></a>teamsAppInstallation 资源类型



安装在[工作组](team.md) [teamsApp](teamsapp.md) 。 应用程序一部分的任何 bot 将成为应用程序添加到任何工作组的一部分。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列表应用程序](../api/teamsappinstallation-list.md) | [teamsAppInstallation](teamsapp.md) | 列出了安装团队中的应用程序。|
|[添加应用程序](../api/teamsappinstallation-add.md) | [teamsAppInstallation](teamsapp.md) | 将 （安装） 添加到团队应用程序。|
|[删除应用程序](../api/teamsappinstallation-delete.md) | 无 | 删除 （卸载） 从团队应用程序。|
|[升级的应用程序](../api/teamsappinstallation-delete.md) | 无 | 升级到最新版本的应用程序。|

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| ID                  | string   | 唯一的 id (不团队 appid)。 |

## <a name="relationships"></a>Relationships

| 关系   | 类型    | Description |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| 安装应用程序。 |
|teamsAppDefinition|[teamsAppDefinition](teamsapp.md)| 此版本的应用程序的详细信息。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a>另请参阅

- [teamsApp](teamsapp.md)
- [teamsAppDefinition](teamsappdefinition.md)
- [teamsTab](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

