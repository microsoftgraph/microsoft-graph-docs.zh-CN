---
title: governancePermission 资源类型
description: '表示 governanceSubject 对特定 governanceResource 具有的访问权限。  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: b88900882ecceabcfe5101aa4564b88116df605f
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397951"
---
# <a name="governancepermission-resource-type"></a>governancePermission 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

表示 [governanceSubject](../resources/governancesubject.md) 对特定 [governanceResource](../resources/governanceresource.md) 具有的访问权限。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accessLevel|String|访问级别。 有效值： ``None``、 ``UserRead``、 ``AdminRead``和 ``AdminReadWrite``.|
|isActive|Boolean|指示请求方是否具有访问级别的任何活动角色分配。|
|isEligible|Boolean|指示请求者是否具有访问级别的任何符合条件的角色分配。|

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


