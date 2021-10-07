---
title: educationSubmissionResource 资源类型
description: 用于提交的资源的包装器。
author: dipakboyed
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ed2d33a9da889925cad08f91b99cc2b2c0c47113
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220477"
---
# <a name="educationsubmissionresource-resource-type"></a>educationSubmissionResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于提交的资源的包装器。 如果从工作分配复制了工作分配资源，包装器会添加一个指向该分配资源的指针。  


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出资源](../api/educationsubmission-list-resources.md) | [educationSubmissionResource](educationsubmissionresource.md) 对象 |返回 **educationSubmissionResource 对象** 的列表。|
|[获取 educationSubmissionResource](../api/educationsubmissionresource-get.md) | [educationSubmissionResource](educationsubmissionresource.md) |读取 **educationSubmissionResource 对象的属性和** 关系。|
|[Delete](../api/educationsubmissionresource-delete.md) | 无 |删除 **educationSubmissionResource** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignmentResourceUrl|String|指向从其中复制此资源的分配的指针。 如果为空，则学生已上传资源。|
|id|字符串| 只读。|
|resource|[educationResource](educationresource.md)|Resource 对象。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionResource"
}-->

```json
{
  "assignmentResourceUrl": "String",
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


