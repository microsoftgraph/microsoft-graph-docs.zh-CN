---
title: educationFormResource 资源类型
description: educationResource 的子类。 此资源是窗体。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3f2747d94c80732091db06294b26546afc567e03
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334253"
---
# <a name="educationformresource-resource-type"></a>educationFormResource 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[educationResource](educationresource.md)的子类。 此资源是窗体。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|originalFormId|String|表单的原始 id。|
|formId|String|表单的 Id。|
|isGroupForm|Boolean|表单是否属于类组。|
|viewUrl|String|表单的学生 URL。|
|viewUrl|String|表单的学生 URL。|
|editUrl|String|表单的教师 URL。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFormResource"
}-->

```json
{
  "originalFormId": "String",
  "formId": "String",
  "isGroupForm": "Boolean",
  "viewUrl": "String",
  "editUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFormResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
