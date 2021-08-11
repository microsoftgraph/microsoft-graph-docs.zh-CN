---
title: educationAssignmentIndividualRecipient 资源类型
description: 在 assignment.assignTo 属性内使用。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4d5f01d3532e6b0022c10947ea36b19c2152fb36409a27cf58898006f5f016ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202425"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a>educationAssignmentIndividualRecipient 资源类型

命名空间：microsoft.graph

在 [assignment.assignTo 属性内](educationassignment.md) 使用。 设置为单个收件人列表时，课堂中选定的学生将在作业发布时收到提交对象。

此资源是 [educationAssignmentRecipient 的子类](educationassignmentrecipient.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|recipients|String collection|收件人的 ID 集合。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentIndividualRecipient"
}-->

```json
{
  "recipients": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


