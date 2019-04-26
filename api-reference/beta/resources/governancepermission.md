---
title: governancePermission 资源类型
description: '表示 governanceSubject 对特定 governanceResource 的访问权限。  '
localization_priority: Normal
ms.openlocfilehash: 2f6be4bdc502f829b1dcfd991d1c2ae6130dea8a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340180"
---
# <a name="governancepermission-resource-type"></a>governancePermission 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[governanceSubject](../resources/governancesubject.md)对特定[governanceResource](../resources/governanceresource.md)的访问权限。  


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accessLevel|String|访问级别。 有效值: ``None``、 ``UserRead`` ``AdminRead``、和。 ``AdminReadWrite``|
|isActive|Boolean|指示请求者是否具有访问级别的任何活动角色分配。|
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
