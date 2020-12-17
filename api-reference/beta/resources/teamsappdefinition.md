---
title: teamsAppDefinition 资源类型
description: teamsApp 的一个版本的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6b5fd771d1fb38de5354c74778f5eae798ccc91e
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706113"
---
# <a name="teamsappdefinition-resource-type"></a>teamsAppDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

teamsApp 版本 [的详细信息](teamsapp.md)。

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 唯一 id (不是 teams appid) 。 |
| teamsAppId          | string   | Teams 应用清单中的 ID。 |
| publishingState| string|特定版本的 Teams 应用的已发布状态。 可能的值是：</br>`submitted` — Teams 应用的特定版本已提交，正在审查中。 </br>`published`  — 发布特定版本的 Teams 应用的请求已由管理员批准并发布。 </br> `rejected` — 管理员拒绝了发布特定版本的 Teams 应用的请求。 |
| azureADAppId        | string   | Teams WebApplicationInfo.id清单中的设置。 |
| displayName         | string   | 应用开发人员提供的应用的名称。 |
| version             | string   | 应用程序的版本号。 |

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
  "displayName": "Test App",
  "version": "1.0.0"
}
```

## <a name="see-also"></a>另请参阅

- [teamsApp](teamsapp.md)
- [teamsAppInstallation](teamsappinstallation.md)
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


