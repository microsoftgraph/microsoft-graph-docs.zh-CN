---
title: managementActionTenantDeploymentStatus 资源类型
description: 表示管理操作租户级别的部署状态。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: c06857bcdf492dc9779768df6fe09d08a6ec87b7
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860573"
---
# <a name="managementactiontenantdeploymentstatus-resource-type"></a>managementActionTenantDeploymentStatus 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示管理操作租户级别的部署状态。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managementActionTenantDeploymentStatus](../api/managedtenants-managedtenant-list-managementactiontenantdeploymentstatuses.md)|[microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) 集合|获取 [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) 对象及其属性的列表。|
|[获取 managementActionTenantDeploymentStatus](../api/managedtenants-managementactiontenantdeploymentstatus-get.md)|[microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md)|读取 [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) 对象的属性和关系。|
|[changeDeploymentStatus](../api/managedtenants-managementactiontenantdeploymentstatus-changedeploymentstatus.md)|[microsoft.graph.managedTenants.managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md)|更改管理操作部署状态。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|租户级别部署状态的唯一标识符。 必需。 只读。|
|statuses|[microsoft.graph.managedTenants.managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) 集合|管理操作的每个实例的部署状态集合。 可选。|
|tenantGroupId|String|与管理操作关联的租户组的标识符。 必需。 只读。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。 必需。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementActionTenantDeploymentStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionTenantDeploymentStatus",
  "id": "String (identifier)",
  "tenantGroupId": "String",
  "tenantId": "String",
  "statuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
    }
  ]
}
```
