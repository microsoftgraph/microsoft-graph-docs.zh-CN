---
title: delegatedAdminAccessDetails 资源类型
description: 表示 Microsoft 合作伙伴通过委派管理员关系和委派管理员访问权限分配在客户租户中具有的管理角色。
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a817e2f0814c19c519475d6fe4c049036ca8c3d2
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589615"
---
# <a name="delegatedadminaccessdetails-resource-type"></a>delegatedAdminAccessDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Microsoft 合作伙伴通过委派管理员关系和委派管理员访问权限分配在客户租户中具有的管理角色。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|unifiedRoles|[unifiedRole](../resources/unifiedrole.md) 集合|在客户租户中分配 Microsoft 合作伙伴的目录角色。|

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

