---
title: targetResourceGroup 资源类型
description: '指示由于审核活动受影响的组的类型。 包括与 Azure AD 的统一组类似的值 '
localization_priority: Normal
ms.openlocfilehash: 2cc7e0adb1a93394b64375d05dfb6a6e349bac55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851182"
---
# <a name="targetresourcegroup-resource-type"></a>targetResourceGroup 资源类型
指示由于审核活动受影响的组的类型。 包括与 Azure AD 的统一组类似的值 



## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|groupType|字符串| 可取值为：`unifiedGroups`、`azureAD`、`unknownFutureValue`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceGroup"
}-->

```json
{
  "groupType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
