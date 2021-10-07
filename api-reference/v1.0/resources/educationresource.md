---
title: educationResource 资源类型
description: 系统中所有资源对象的基类。
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 17accd1da2d273878297ddba1c6e8d9caac8f46b
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220540"
---
# <a name="educationresource-resource-type"></a>educationResource 资源类型

命名空间：microsoft.graph

educationExcelResource、educationFileResource、educationLinkResource、educationPowerPointResource、educationWordResource、educationMediaResource[](../resources/educationmediaresource.md)和[](../resources/educationlinkresource.md)[educationExternalResource 的基类](../resources/educationexternalresource.md)。 [](../resources/educationexcelresource.md) [](../resources/educationfileresource.md) [](../resources/educationpowerpointresource.md) [](../resources/educationwordresource.md)

educationResource 与作业和/或[](educationassignment.md)提交相关联，它[](educationsubmission.md)表示正在提供或提交的学习对象。 不能直接实例化资源;您必须创建一个表示所使用的资源类型的子类。

此资源存储所有资源类型的通用属性。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|创建资源的人。|
|createdDateTime|DateTimeOffset|创建资源的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|displayName|String|资源的显示名称。|
|lastModifiedBy|[identitySet](identityset.md)|最后一个修改资源的用户。|
|lastModifiedDateTime|DateTimeOffset|上次修改资源的时间。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|

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


