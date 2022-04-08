---
title: delegatedAdminAccessDetails 资源类型
description: 表示 Microsoft 合作伙伴通过委派的管理员关系和委派的管理员访问分配在客户租户中具有的管理角色。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: c67f7792ea1124228a23fdc5b642dc3de47739a8
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704163"
---
# <a name="delegatedadminaccessdetails-resource-type"></a>delegatedAdminAccessDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Microsoft 合作伙伴通过委派的管理员关系和委派的管理员访问分配在客户租户中具有的管理角色。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|unifiedRoles|[unifiedRole](../resources/unifiedrole.md) 集合|Microsoft 合作伙伴在客户租户中分配的目录角色。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.delegatedAdminAccessDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminAccessDetails",
  "unifiedRoles": [
    {
      "@odata.type": "microsoft.graph.unifiedRole"
    }
  ]
}
```

