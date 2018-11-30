---
title: extensionSchemaProperty 资源类型
description: 使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 schemaExtension 定义的一部分。
ms.openlocfilehash: f699ccebefc849a7bf9cacc6dbda61cbcbb9896d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043092"
---
# <a name="extensionschemaproperty-resource-type"></a>extensionSchemaProperty 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 [schemaExtension](schemaextension.md) 定义的一部分。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|name|字符串| 架构扩展的一部分定义的强类型属性的名称。|
|type|String| 被定义为架构扩展组成部分的属性的类型。允许的值为 *Binary、Boolean、DateTime、Integer* 或 *String*。请参阅下表获取更多详细信息。|

#### <a name="supported-property-data-types"></a>受支持的属性数据类型 
在架构扩展中定义属性时，支持以下数据类型：

| 属性类型 | 备注 |
|-------------|------------|
| Binary | 最多 256 字节。 |
| Boolean | 不支持消息、活动和帖子。 |
| 日期时间 | 必须以 ISO 8601 格式进行指定。存储为 UTC 格式。 |
| 整数 | 32 位值。不支持消息、活动和帖子。 |
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