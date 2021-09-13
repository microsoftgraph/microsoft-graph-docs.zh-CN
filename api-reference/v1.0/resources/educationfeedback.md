---
title: educationFeedback 资源类型
description: 从教师到学生的反馈。
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 795302823311169b11bd57ae89f252abba833ef0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036681"
---
# <a name="educationfeedback-resource-type"></a>educationFeedback 资源类型

命名空间：microsoft.graph

从教师到学生的反馈。 

此属性表示反馈的文本部分以及提供反馈的人。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|feedbackBy|[identitySet](identityset.md)|创建反馈的用户。|
|feedbackDateTime|DateTimeOffset|提供反馈的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|text|[itemBody](itembody.md)|反馈。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedback"
}-->

```json
{
  "feedbackBy": {"@odata.type": "microsoft.graph.identitySet"},
  "feedbackDateTime": "String",
  "text": {"@odata.type": "microsoft.graph.itemBody"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


