---
title: governancePermission 资源类型
description: '表示对特定 governanceResource governanceSubject 具有访问权限。  '
localization_priority: Normal
ms.openlocfilehash: 9b6e920d92d7010fb325be05cf0b645f9b8d81cd
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570720"
---
# <a name="governancepermission-resource-type"></a>governancePermission 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示对特定[governanceResource](../resources/governanceresource.md) [governanceSubject](../resources/governancesubject.md)具有访问权限。  


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accessLevel|String|访问级别。 有效值： ``None``， ``UserRead``， ``AdminRead``，和``AdminReadWrite``。|
|isActive|布尔值|指示如果请求者有任何主动角色分配访问级别。|
|isEligible|布尔值|指示请求者是否具有任何访问级别的合格的角色分配。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governancePermission"
}-->
```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancepermission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
