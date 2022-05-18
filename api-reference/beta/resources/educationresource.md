---
title: educationResource 资源类型
description: 系统中所有资源对象的基类。
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1af5cb6ae12eb435b6335d902430fdbc717fcd25
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461364"
---
# <a name="educationresource-resource-type"></a>educationResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

教育 [ExcelResource](../resources/educationexcelresource.md)、 [educationFileResource](../resources/educationfileresource.md)、 [educationLinkResource](../resources/educationlinkresource.md)、 [educationPowerPointResource](../resources/educationpowerpointresource.md)、 [educationWordResource](../resources/educationwordresource.md)、 [educationMediaResource](../resources/educationmediaresource.md)、 [educationExternalResource](../resources/educationexternalresource.md) 和 [educationTeamsAppResource](../resources/educationteamsappresource.md) 的基类。

educationResource 与分配和/或提交相关联，该 [作业](educationassignment.md) 和/或 [提交](educationsubmission.md)表示正在分发或上交的学习对象。 不能直接实例化资源;必须创建一个子类，该子类将表示正在使用的资源类型。

此资源存储所有资源类型的常见属性。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Who创建了资源。|
|createdDateTime|创建资源的时间。  DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|displayName|String|显示资源的名称。|
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


