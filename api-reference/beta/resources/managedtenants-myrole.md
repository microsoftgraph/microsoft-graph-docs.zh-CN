---
title: myRole 资源类型
description: 表示托管租户的已登录用户的角色分配。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3607702c037155efef1e0353b3551ba79f3eda9c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096353"
---
# <a name="myrole-resource-type"></a>myRole 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托 [管租户](../resources/managedtenants-tenant.md)的已登录用户的角色分配。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 myRoles](../api/managedtenants-managedtenant-list-myroles.md)|[microsoft.graph.managedTenants.myRole](../resources/managedtenants-myrole.md) 集合|获取已登录用户通过托 [管租户](../resources/managedtenants-tenant.md)之间的委托关系所具有的角色。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|assignments|[microsoft.graph.managedTenants.roleAssignment](../resources/managedtenants-roleassignment.md) 集合|托 [管租户](../resources/managedtenants-tenant.md)的角色分配集合。|
|tenantId|String|托管租户的Azure Active Directory[租户](../resources/managedtenants-tenant.md)标识符。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.myRole",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.myRole",
  "assignments": [
    {
      "@odata.type": "microsoft.graph.managedTenants.roleAssignment"
    }
  ],
  "tenantId": "String"
}
```
