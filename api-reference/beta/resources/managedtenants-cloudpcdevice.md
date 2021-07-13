---
title: cloudPcDevice 资源类型
description: 表示属于给定托管租户的云电脑设备。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 57eabb6720987a8a9bfca4c18e283057848b65cf
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402071"
---
# <a name="cloudpcdevice-resource-type"></a>cloudPcDevice 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示属于给定托管租户的云电脑设备。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 cloudPcDevices](../api/managedtenants-managedtenant-list-cloudpcdevices.md)|[microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) 集合|获取 [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) 对象及其属性的列表。|
|[获取 cloudPcDevice](../api/managedtenants-cloudpcdevice-get.md)|[microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md)|读取 [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|cloudPcStatus|String|云电脑的状态。 可取值为：`notProvisioned`、`provisioning`、`provisioned`、`upgrading`、`inGracePeriod`、`deprovisioning` 或 `failed`。 必填。 只读。|
|displayName|String|云显示名称应用。 必填。 只读。|
|id|String|云电脑的唯一标识符。 必填。 只读。|
|lastRefreshedDateTime|DateTimeOffset|实体上次在多租户管理平台中更新的日期和时间。 必填。 只读。|
|managedDeviceId|String|云电脑的托管设备标识符。 可选。 只读。|
|managedDeviceName|String|托管设备显示名称云电脑。 可选。 只读。|
|provisioningPolicyId|String|云电脑的预配策略标识符。 必填。 只读。|
|servicePlanName|String|云电脑的服务计划名称。 必填。 只读。|
|tenantDisplayName|String|托管显示名称租户的租户。 必填。 只读。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。 必填。 只读。|
|userPrincipalName|String|用户主体名称 (分配给) 电脑的用户的 UPN 名称。 必填。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcDevice",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcDevice",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "userPrincipalName": "String",
  "servicePlanName": "String",
  "cloudPcStatus": "String",
  "provisioningPolicyId": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
