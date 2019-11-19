---
title: externalFile 资源类型
description: 通过 Microsoft Search 连接编制索引的文件。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c3e51c27985927f5ea71f8ca618c4055a609fc06
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703747"
---
# <a name="externalfile-resource-type"></a>externalFile 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过 Microsoft Search[连接](externalconnection.md)编制索引的项目。 此类型派生自[externalItem](externalitem.md)类型。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>方法

| 方法                                                        | 返回类型  | 说明 |
|:--------------------------------------------------------------|:-------------|:--|
| [创建 externalFile](../api/externalconnection-put-items.md) | externalFile | 创建 externalFile。 |
| [更新 externalFile](../api/externalitem-update.md)          | externalFile | 更新 externalFile。 |
| [删除](../api/externalitem-delete.md)                       | 无         | 删除 externalFile。 |

## <a name="properties"></a>属性

| 属性         | 类型                     | 说明                    |
|:-----------------|:-------------------------|:-------------------------------|
| acl              | [acl](acl.md)集合 | 一组访问控制项。 每个条目指定向用户或组授予的访问权限。 必需。 |
| 内容          | String                   | 项目内容的纯文本表示形式。 此属性中的文本为全文检索的文本。 可选。 |
| id               | String                   | 开发人员提供的包含[externalConnection](externalconnection.md)中的项的唯一 ID。 必须为字母数字，最多为128个字符。 必需。 |
| createdBy        | String                   | 创建文件的用户的名称。 |
| createdDateTime  | DateTimeOffset           | 创建文件的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'` |
| 扩展        | String                   | 文件扩展名。            |
| lastModifiedBy   | String                   | 上次修改文件的用户的名称。 |
| modifiedDateTime | DateTimeOffset           | 上次修改文件的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'` |
| name             | 字符串                   | 文件名。 必需。       |
| size             | Int64                    | 文件的大小（以字节为单位）。 |
| title            | String                   | 文件的标题。         |
| url              | String                   | 用于访问文件的 URL。 必需。 |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalFile",
  "baseType": "microsoft.graph.externalItem"
}-->

```json
{
  "acl": [{"@odata.type": "microsoft.graph.acl"}],
  "content": "String",
  "id": "String (identifier)",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "extension": "String",
  "lastModifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "title": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
