---
title: educationFileResource 资源类型
description: educationResource 子类，表示与分配或提交关联的文件对象。  在这种情况下，该文件不是 Word、Excel 等 (特殊文件之一) 但该文件在系统中没有特殊处理。 文件资源必须存储在与此资源附加到的分配或提交关联的 **resourceFolder** 中。
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 325fc7beec6eeb482cb19cd1c56eebf144b41cf7
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684688"
---
# <a name="educationfileresource-resource-type"></a>educationFileResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[educationResource](educationresource.md) 子类，表示与分配或提交关联的文件对象。  在这种情况下，该文件不是 Word、Excel 等 (特殊文件之一) 但该文件在系统中没有特殊处理。 文件资源必须存储在与此资源附加到的分配或提交关联的 **resourceFolder** 中。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|fileUrl|String|文件资源磁盘上的位置。|
|createdBy|String|创建此对象的用户的显示名称。|
|createdDateTime|DateTimeOffset|添加重索的日期时间。|
|displayName|string|资源的显示名称。|
|lastModifiedBy|[identitySet](identityset.md)|最后一个修改资源的用户。|
|lastModifiedDateTime|DateTimeOffset|上次修改资源的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
}-->

```json
{
  "fileUrl": "String",
  "createdBy": "String (User)",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": "String (User)",
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


