---
title: educationSubmissionResource 资源类型
description: '资源周围的包装，用于提交。 如果从分配中复制了该包装，则包装将添加指向该工作分配资源的指针。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 329bab18d90412ec8cc06b12106e0be4f1b46935
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979561"
---
# <a name="educationsubmissionresource-resource-type"></a>educationSubmissionResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

资源周围的包装，用于提交。 如果从分配中复制了该包装，则包装将添加指向该工作分配资源的指针。  


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 educationSubmissionResource](../api/educationsubmissionresource-get.md) | [educationSubmissionResource](educationsubmissionresource.md) |读取 **educationSubmissionResource** 对象的属性和关系。|
|[删除](../api/educationsubmissionresource-delete.md) | 无 |删除 **educationSubmissionResource** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignmentResourceUrl|String|指向从其复制此资源的工作分配的指针。 如果为 null，则学生上传了资源。|
|id|String| 只读。|
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


