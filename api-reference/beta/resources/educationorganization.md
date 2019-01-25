---
title: educationOrganization 资源类型
description: '用于模型之间的教育扇区中的不同组织类型通用性抽象实体。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 122717952781cd8effe415fb01b07ec9bf71143d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507472"
---
# <a name="educationorganization-resource-type"></a>educationOrganization 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于模型之间的教育扇区中的不同组织类型通用性抽象实体。  

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|String| 组织说明。|
|displayName|String| 组织的显示名称。|
|externalSource|string| 从在其中创建此组织的源。 可取值为：`sis`、`manual`、`unknownFutureValue`。|

## <a name="relationships"></a>Relationships
无。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationorganization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
