---
title: governancePermission 资源类型
description: '表示 governanceSubject 对特定 governanceResource 具有的访问权限。  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: b4244335bba57c9ff5200099520e2e0b2a5e98c2
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510406"
---
# <a name="governancepermission-resource-type"></a>governancePermission 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

表示 [governanceSubject](../resources/governancesubject.md) 对特定 [governanceResource 具有的访问权限](../resources/governanceresource.md)。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accessLevel|String|访问级别。 有效值：、``None````UserRead``、``AdminRead``和 ``AdminReadWrite``。|
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


