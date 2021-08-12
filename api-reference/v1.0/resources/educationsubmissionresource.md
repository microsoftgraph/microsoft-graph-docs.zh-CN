---
title: educationSubmissionResource 资源类型
description: 用于提交的资源的包装器。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b24f1ea91691dd66d66848abcdb0069e9a25e4865f18f05b7682d2fb4a8f3d88
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141747"
---
# <a name="educationsubmissionresource-resource-type"></a>educationSubmissionResource 资源类型

命名空间：microsoft.graph

用于提交的资源的包装器。 

如果从工作分配复制了工作分配资源，包装器会添加一个指向该分配资源的指针。  


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 educationSubmissionResource](../api/educationsubmissionresource-get.md) | [educationSubmissionResource](educationsubmissionresource.md) |读取 **educationSubmissionResource 对象的属性和** 关系。|
|[删除](../api/educationsubmissionresource-delete.md) | 无 |删除 **educationSubmissionResource** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignmentResourceUrl|String|指向从其中复制此资源的分配的指针。 如果为空，则学生已上传资源。|
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


