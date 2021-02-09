---
title: externalItem 资源类型
description: 添加到 Microsoft Graph 连接中的项。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 63f0285427a17280169d31a35c3a622d38a6a8c6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161698"
---
# <a name="externalitem-resource-type"></a>externalItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

添加到 Microsoft Graph 连接 [中的项](externalconnection.md)。 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>方法

| 方法                                                        | 返回类型                     | 说明 |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [创建 externalItem](../api/externalconnection-put-items.md) | [externalItem](externalitem.md) | 创建 externalItem。 |
| [获取 externalItem](../api/externalitem-get.md)                | [externalItem](externalitem.md) | 获取 externalItem。    |
| [更新 externalItem](../api/externalitem-update.md)          | [externalItem](externalitem.md) | 更新 externalItem。 |
| [删除 externalItem](../api/externalitem-delete.md)          | 无                            | 删除 externalItem。 |

## <a name="properties"></a>属性

| 属性   | 类型                     | 说明                          |
|:-----------|:-------------------------|:-------------------------------------|
| acl        | [acl](acl.md) 集合 | 访问控制项数组。 每个条目指定授予用户或组的访问权限。 必需。 |
| content    | [externalItemContent](externalitemcontent.md) | 项目内容的纯文本表示形式。 此属性中的文本是全文索引。 可选。 |
| id         | String                   | 开发人员提供包含外部Connection 中的项的唯一[ID。](externalconnection.md) 必须为字母数字，最多为 128 个字符。 必需。 |
| properties | Object                   | 具有项目属性的属性包。 属性必须符合为[externalConnection](externalconnection.md)定义的架构。 [](schema.md) 必填。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItem",
  "keyProperty": "id"
}-->

```json
{
  "acl": [{"@odata.type": "microsoft.graph.acl"}],
  "content": {"@odata.type": "microsoft.graph.externalItemContent"},
  "id": "String (identifier)",
  "properties": "Object"
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
    "Error: microsoft.graph.externalItem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->
