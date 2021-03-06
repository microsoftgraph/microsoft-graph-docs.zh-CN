---
title: educationResource 资源类型
description: 系统中所有资源对象的超级类。 资源与工作分配和/或 **提交** 相关联，它表示正在学习的对象
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f82274782f84204be288c67365288891f64fedf6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440944"
---
# <a name="educationresource-resource-type"></a>educationResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

系统中所有资源对象的超级类。 资源与工作分配和/或 **提交** 相关联，它表示要分配或提交的学习对象。 不能直接实例化资源;您必须创建一个表示所使用的资源类型的子类。

此资源存储所有资源类型的通用属性。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Who创建了资源。|
|createdDateTime|创建资源的时间。  DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|displayName|String|资源的显示名称。|
|lastModifiedBy|[identitySet](identityset.md)|Who是最后一个修改资源的用户。|
|lastModifiedDateTime|DateTimeOffset|上次修改资源的时间。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationResource"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


