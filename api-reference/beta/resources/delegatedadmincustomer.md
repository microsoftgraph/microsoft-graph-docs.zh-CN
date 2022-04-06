---
title: delegatedAdminCustomer 资源类型
description: 表示与 Microsoft 合作伙伴具有委派管理员关系的客户。
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b7ac3c580ab566565d99f7c7c542e2bee0f0bcc3
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589754"
---
# <a name="delegatedadmincustomer-resource-type"></a>delegatedAdminCustomer 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表Azure AD Microsoft 合作伙伴的客户且与 Microsoft 合作伙伴具有委派管理员关系的组织。 当合作伙伴与客户之间至少存在一个委派管理员关系时，系统会自动创建此对象，当不存在更多活动关系时，此对象将被删除。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 delegatedAdminCustomers](../api/tenantrelationship-list-delegatedadmincustomers.md)|[delegatedAdminCustomer](delegatedadmincustomer.md) 集合|获取 **delegatedAdminCustomer** 对象及其属性的列表。|
|[获取 delegatedAdminCustomer](../api/delegatedadmincustomer-get.md)|[delegatedAdminCustomer](delegatedadmincustomer.md)|读取 **delegatedAdminCustomer** 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|客户Azure AD 显示名称的租户。 只读。 支持 `$orderBy`。 |
|id|String|客户Azure AD分配的唯一标识符。 只读。 继承自 [entity](../resources/entity.md)。|
|tenantId|String|客户Azure AD的租户 ID。 只读。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|serviceManagementDetails|[delegatedAdminServiceManagementDetail](delegatedadminservicemanagementdetail.md) 集合|包含由委派管理的客户租户中服务的管理详细信息。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminCustomer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminCustomer",
  "id": "String (identifier)",
  "tenantId": "String",
  "displayName": "String"
}
```
