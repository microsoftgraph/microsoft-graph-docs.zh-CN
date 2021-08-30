---
title: teamwork 资源类型
description: 可供组织使用的 Microsoft Teams 功能的容器。
author: akjo
doc_type: resourcePageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 012286f43a6ab31f29062317077042ce43b587e9
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695901"
---
# <a name="teamwork-resource-type"></a>teamwork 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可供组织使用的 Microsoft Teams 功能范围的容器。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|id|string| 唯一标识符。 |

## <a name="relationships"></a>关系

| 关系 | 类型 | 说明 |
|:---------------|:--------|:----------|
|installedApps|[teamsAppInstallation](teamsappinstallation.md) 集合|此用户的个人范围内安装的应用。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamwork",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}

```

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

## <a name="see-also"></a>另请参阅

- [userTeamwork 资源类型](userteamwork.md)


