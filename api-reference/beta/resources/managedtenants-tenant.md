---
title: 租户资源类型
description: 表示与管理实体关联的租户。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: ee4bd57aa4e7fa2ea15c86376389d3b6e12198ea
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402396"
---
# <a name="tenant-resource-type"></a>租户资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与管理实体关联的租户。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出租户](../api/managedtenants-managedtenant-list-tenants.md)|[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md) 集合|获取租户对象 [及其](../resources/managedtenants-tenant.md) 属性的列表。|
|[获取租户](../api/managedtenants-tenant-get.md)|[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|读取租户对象的属性 [和](../resources/managedtenants-tenant.md) 关系。|
|[offboardTenant](../api/managedtenants-tenant-offboardtenant.md)|[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|从多租户管理平台注销租户。|
|[resetTenantOnboardingStatus](../api/managedtenants-tenant-resettenantonboardingstatus.md)|[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|使用多租户管理平台重置租户载入状态。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|contract|[microsoft.graph.managedTenants.tenantContract](../resources/managedtenants-tenantcontract.md)|租户与管理实体的关系详细信息。|
|createdDateTime|DateTimeOffset|在多租户管理平台中创建租户的日期和时间。 可选。 只读。|
|displayName|String|租户的显示名称。 必填。 只读。|
|id|String|租户Azure Active Directory租户标识符。 必填。 只读。|
|lastUpdatedDateTime|DateTimeOffset|在多租户管理平台中上次更新租户的日期和时间。 可选。 只读。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。 可选。 只读。|
|tenantStatusInformation|[microsoft.graph.managedTenants.tenantStatusInformation](../resources/managedtenants-tenantstatusinformation.md)|租户的载入状态信息。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenant",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenant",
  "id": "String (identifier)",
  "tenantId": "String",
  "displayName": "String",
  "contract": {
    "@odata.type": "microsoft.graph.managedTenants.tenantContract"
  },
  "tenantStatusInformation": {
    "@odata.type": "microsoft.graph.managedTenants.tenantStatusInformation"
  },
  "lastUpdatedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)"
}
```
