---
title: educationAssignmentIndividualRecipient 资源类型
description: '在 assignTo 属性中使用。 当设置为 "单个收件人列表" 时, 课程中的 "选定学生" 将 '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7408382cadcb53d857bb36b06702f7857d64a8f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006449"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a>educationAssignmentIndividualRecipient 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[assignTo](educationassignment.md)属性中使用。 如果设置为 "单个收件人列表", 则在发布工作分配时, 类中的所选学生将收到提交对象。

此资源是[educationAssignmentRecipient](educationassignmentrecipient.md)的子类。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|recipients|String collection|收件人的 id 的集合。|

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
