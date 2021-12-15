---
title: bookingStaffMemberBase 资源类型
description: Bookings 员工成员的抽象基本类型。
author: davisjms
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 17d13e80cf61e1cc885b07666708c9f8f479a385
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526506"
---
# <a name="bookingstaffmemberbase-resource-type"></a>bookingStaffMemberBase 资源类型

命名空间：microsoft.graph

Bookings 员工成员的抽象基本类型。

[bookingStaffMember 的基本类型](bookingstaffmember.md)。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|员工 ID。 继承自 [实体](../resources/entity.md)。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingStaffMemberBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingStaffMemberBase",
  "id": "String (identifier)"
}
```

