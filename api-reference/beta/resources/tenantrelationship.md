---
title: tenantRelationship 资源类型
description: 表示各种类型的租户关系。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 5873f7b2740b342619755ea3bdda3cdd587837ea
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587306"
---
# <a name="tenantrelationship-resource-type"></a>tenantRelationship 资源类型

命名空间：microsoft.graph

表示各种类型的租户关系。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|delegatedAdminCustomers|[delegatedAdminCustomer](../resources/delegatedadmincustomer.md) 集合|与 Microsoft 合作伙伴具有委派管理员关系的客户。|
|delegatedAdminRelationships|[delegatedAdminRelationship](../resources/delegatedadminrelationship.md) 集合|Microsoft 合作伙伴在客户租户中具有的委派管理权限的详细信息。|
|managedTenants|[microsoft.graph.managedTenants.managedTenant](../resources/managedtenants-managedtenant.md)|可用于与多租户管理平台交互的操作。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tenantRelationship",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tenantRelationship"
}
```
