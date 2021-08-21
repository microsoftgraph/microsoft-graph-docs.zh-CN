---
title: governancePermission 资源类型
description: '表示 governanceSubject 对特定 governanceResource 具有的访问权限。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: c094050f32b020c204d645dfc0c398ad5bfa5d20
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453728"
---
# <a name="governancepermission-resource-type"></a>governancePermission 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [governanceSubject](../resources/governancesubject.md) 对特定 [governanceResource 具有的访问权限](../resources/governanceresource.md)。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accessLevel|String|访问级别。 有效值 ``None`` ``UserRead`` ：、、 ``AdminRead`` 和 ``AdminReadWrite`` 。|
|isActive|Boolean|指示请求程序是否具有访问角色分配活动状态。|
|isEligible|Boolean|指示请求者是否有符合访问角色分配条件。|

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


