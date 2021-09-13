---
title: teamsTab 资源类型
description: 'teamsTab 是固定到团队中 (附加到) 频道的选项卡。 '
ms.localizationpriority: medium
author: AkJo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 66dfa63b09463fac67b95bf4e635d90ffa4348a7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59066973"
---
# <a name="teamstab-resource-type"></a>teamsTab 资源类型

命名空间：microsoft.graph



teamsTab[是固定](../resources/teamstab.md)到 (附加到) 频道的[](channel.md)[选项卡](team.md)。 

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出选项卡](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | 列出固定到频道的选项卡。|
|[获取选项卡](../api/channel-get-tabs.md) | [teamsTab](teamstab.md) | 读取固定到频道的选项卡。|
|[添加选项卡](../api/channel-post-tabs.md) | [teamsTab](teamstab.md) | 将选项卡添加（固定）到频道。|
|[更新选项卡](../api/channel-patch-tabs.md) | [teamsTab](teamstab.md) | 更新选项卡属性。|
|[删除选项卡](../api/channel-delete-tabs.md) | 无 | 从频道中删除（取消固定）选项卡。|


## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|  id              |   string                  |  唯一标识通道选项卡的特定实例的标识符。只读。     |
|  displayName            |   string                  |  选项卡的名称。     |
|  WebUrl          |   string                  |  选项卡实例的深层链接 URL。 只读。     |
|  configuration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  应用于选项卡的自定义设置的容器。只有在设置此属性后，选项卡才被视为已配置。     |

## <a name="relationships"></a>关系

| 关系 | 类型   | 说明 |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | 链接到选项卡的应用程序。这无法在选项卡创建后更改。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a>另请参阅

[配置内置选项卡类型](/graph/teams-configuring-builtin-tabs)

