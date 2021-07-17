---
title: externalItem 资源类型
description: 添加到 Microsoft Graph项。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8660365d5d08d0084066cea3349e841269469241
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467666"
---
# <a name="externalitem-resource-type"></a>externalItem 资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

添加到 Microsoft Graph[项](externalconnectors-externalconnection.md)。

## <a name="methods"></a>方法

| 方法                                                        | 返回类型                     | 说明 |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [创建 externalItem](../api/externalconnectors-externalconnection-put-items.md) | [externalItem](externalconnectors-externalitem.md) | 创建 externalItem。 |
| [获取 externalItem](../api/externalconnectors-externalitem-get.md)                | [externalItem](externalconnectors-externalitem.md) | 获取 externalItem。    |
| [更新 externalItem](../api/externalconnectors-externalitem-update.md)          | [externalItem](externalconnectors-externalitem.md) | 更新 externalItem。 |
| [删除 externalItem](../api/externalconnectors-externalitem-delete.md)          | 无                            | 删除 externalItem。 |

## <a name="properties"></a>属性

| 属性   | 类型                     | 说明                          |
|:-----------|:-------------------------|:-------------------------------------|
| acl        | [microsoft.graph.externalConnectors.acl](externalconnectors-acl.md) 集合 | 访问控制项数组。 每个条目指定授予用户或组的访问权限。 必需项。 |
| content    | [microsoft.graph.externalConnectors.externalItemContent](externalconnectors-externalitemcontent.md) | 项目内容的纯文本表示形式。 此属性中的文本已编制全文索引。 可选。 |
| id         | String                   | 开发人员提供的项目在包含[externalConnection 中的唯一 ID。](externalconnectors-externalconnection.md) 必须为字母数字，最多为 128 个字符。 必需项。 |
| properties | Object                   | 具有项目属性的属性包。 属性必须符合为[externalConnection](externalconnectors-externalconnection.md)定义的架构。 [](externalconnectors-schema.md) 必填。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalItem",
  "keyProperty": "id"
}-->

```json
{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    }
  ],
  "id": "String (identifier)",
  "properties": "Object",
  "content": { "@odata.type": "microsoft.graph.externalConnectors.externalItemContent" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.externalConnectors.externalItem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->
