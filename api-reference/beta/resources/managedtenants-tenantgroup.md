---
title: tenantGroup 资源类型
description: 表示托管租户的逻辑组。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2ab0d97afff68dca7d76b1ad6c4e461ad6af6233
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402272"
---
# <a name="tenantgroup-resource-type"></a>tenantGroup 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托管租户的逻辑组。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 tenantGroups](../api/managedtenants-managedtenant-list-tenantgroups.md)|[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) 集合|获取 [tenantGroup 对象](../resources/managedtenants-tenantgroup.md) 及其属性的列表。|
|[获取 tenantGroup](../api/managedtenants-tenantgroup-get.md)|[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)|读取 [tenantGroup](../resources/managedtenants-tenantgroup.md) 对象的属性和关系。|
|[tenantSearch](../api/managedtenants-tenantgroup-tenantsearch.md)|[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) 集合|跨租户组搜索特定的托管租户。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allTenantsIncluded|布尔|一个标志，指示所有托管租户是否都包含在租户组中。 必填。 只读。|
|displayName|String|租户显示名称的组。 可选。 只读。|
|id|String|租户组的唯一标识符。 必填。 只读。|
|managementActions|[microsoft.graph.managedTenants.managementActionInfo](../resources/managedtenants-managementactioninfo.md) 集合|与租户组关联的管理操作的集合。 可选。 只读。|
|managementIntents|[microsoft.graph.managedTenants.managementIntentInfo](../resources/managedtenants-managementintentinfo.md) 集合|与租户组关联的管理意图的集合。 可选。 只读。|
|tenantIds|字符串集合|托管租户标识符的集合包括在租户组中。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantGroup",
  "id": "String (identifier)",
  "displayName": "String",
  "allTenantsIncluded": "Boolean",
  "tenantIds": [
    "String"
  ],
  "managementIntents": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementIntentInfo"
    }
  ],
  "managementActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementActionInfo"
    }
  ]
}
```
