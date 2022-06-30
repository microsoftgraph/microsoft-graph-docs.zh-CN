---
title: extensionSchemaProperty 资源类型
description: 使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 schemaExtension 定义的一部分。
ms.localizationpriority: medium
author: keylimesoda
ms.prod: extensions
doc_type: resourcePageType
ms.openlocfilehash: e86f97f8bb56214e376ceca8db3b00356561f6a2
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556127"
---
# <a name="extensionschemaproperty-resource-type"></a>extensionSchemaProperty 资源类型

命名空间：microsoft.graph

使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 [schemaExtension](schemaextension.md) 定义的一部分。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|name|String| 被定义为架构扩展组成部分的强类型属性的名称。|
|type|字符串| 定义为架构扩展的一部分的属性的类型。  允许的值为 `Binary`、`Boolean`或 `Integer` `DateTime``String`. 有关更多详细信息，请参阅下表。|

### <a name="supported-property-data-types"></a>受支持的属性数据类型

在架构扩展中定义属性时，支持以下数据类型：

| 属性类型 | 备注 |
|-------------|------------|
| Binary | 最多 256 字节。 |
| Boolean | 不受联系人、邮件、活动和帖子支持。 |
| 日期时间 | 必须以 ISO 8601 格式进行指定。存储为 UTC 格式。 |
| 整数 | 32 位值。 不受联系人、邮件、活动和帖子支持。 |
| 字符串 | 最多 256 个字符。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

