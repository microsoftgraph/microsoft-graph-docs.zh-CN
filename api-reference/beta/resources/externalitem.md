---
title: externalItem 资源类型
description: 添加到 Microsoft Graph 连接的项。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ec2c66c91612738295ac4ba49524593d61ff70e4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193400"
---
# <a name="externalitem-resource-type"></a>externalItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

添加到 Microsoft Graph [连接](externalconnection.md)的项。 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>方法

| 方法                                                        | 返回类型                     | 说明 |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [创建 externalItem](../api/externalconnection-put-items.md) | [externalItem](externalitem.md) | 创建 externalItem。 |
| [获取 externalItem](../api/externalitem-get.md)                | [externalItem](externalitem.md) | 获取 externalItem。    |
| [更新 externalItem](../api/externalitem-update.md)          | [externalItem](externalitem.md) | 更新 externalItem。 |
| [删除 externalItem](../api/externalitem-delete.md)          | 无                            | 删除 externalItem。 |

## <a name="properties"></a>属性

| 属性   | 类型                     | 描述                          |
|:-----------|:-------------------------|:-------------------------------------|
| acl        | [acl](acl.md) 集合 | 一组访问控制项。 每个条目指定向用户或组授予的访问权限。 必需。 |
| content    | [externalItemContent](externalitemcontent.md) | 项目内容的纯文本表示形式。 此属性中的文本为全文检索的文本。 可选。 |
| id         | 字符串                   | 开发人员提供的包含 [externalConnection](externalconnection.md)中的项的唯一 ID。 必须为字母数字，最多为128个字符。 必需。 |
| properties | Object                   | 包含项属性的属性包。 属性必须符合为[externalConnection](externalconnection.md)定义的[架构](schema.md)。 必填。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItem",
  "baseType": "",
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
