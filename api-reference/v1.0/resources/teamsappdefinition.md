---
title: teamsAppDefinition 资源类型
description: 表示 teamsApp 的一个版本的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8a43083e1f7fb717e2d54caef4017aeae97d9392
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625931"
---
# <a name="teamsappdefinition-resource-type"></a>teamsAppDefinition 资源类型

命名空间：microsoft.graph

表示 [teamsApp](teamsapp.md)版本的详细信息。

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 唯一 ID (Teams 应用 ID) 。 |
| teamsAppId          | string   | Teams 应用清单中的 ID。 |
| publishingState| string|特定版本的 Teams 应用的已发布状态。 可能的值是：</br>`submitted` — Teams 应用的特定版本已提交，正在审查中。 </br>`published`  — 发布特定版本的 Teams 应用的请求已由管理员批准，并且该应用已发布。 </br> `rejected` — 管理员拒绝了发布特定版本的 Teams 应用的请求。 |
| displayName         | string   | 应用开发人员提供的应用的名称。 |
| version             | string   | 应用程序的版本号。 |
| shortDescription    | string   | 应用程序的简短说明。 |
| 说明         | string   | 应用程序的详细说明。 |

## <a name="relationships"></a>关系

| 关系 | 类型   | 说明 |
|:---------------|:--------|:----------|
|bot|[teamworkBot](teamworkbot.md) | Teams 应用清单中指定的自动程序的详细信息。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "string",
  "version": "string"
}
```

## <a name="see-also"></a>另请参阅

- [teamsApp](teamsapp.md)
- [teamsAppInstallation](teamsappinstallation.md)
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

