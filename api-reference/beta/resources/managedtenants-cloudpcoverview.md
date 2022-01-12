---
title: cloudPcOverview 资源类型
description: 表示给定托管租户的云电脑概述。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 1eb4349c16a529c1ae3a8a9f57c221dd129ba5cc
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61795555"
---
# <a name="cloudpcoverview-resource-type"></a>cloudPcOverview 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示给定托管租户的云电脑概述。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 cloudPcOverviews](../api/managedtenants-managedtenant-list-cloudpcsoverview.md)|[microsoft.graph.managedTenants.cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) 集合|获取 [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) 对象及其属性的列表。|
|[获取 cloudPcOverview](../api/managedtenants-cloudpcoverview-get.md)|[microsoft.graph.managedTenants.cloudPcOverview](../resources/managedtenants-cloudpcoverview.md)|读取 [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|云电脑概述的唯一标识符。 必需。 只读。|
|lastRefreshedDateTime|DateTimeOffset|实体上次在多租户管理平台中更新的日期和时间。 可选。 只读。|
|numberOfCloudPcConnectionStatusFailed|Int32|状态为 的云电脑连接数 `failed` 。 可选。 只读。|
|numberOfCloudPcConnectionStatusPassed|Int32|状态为 的云电脑连接数 `passed` 。 可选。 只读。|
|numberOfCloudPcConnectionStatusPending|Int32|状态为 的云电脑连接数 `pending` 。 可选。 只读。|
|numberOfCloudPcConnectionStatusRunning|Int32|状态为 的云电脑连接数 `running` 。 可选。 只读。|
|numberOfCloudPcConnectionStatusUnkownFutureValue|Int32|状态为 的云电脑连接数 `unknownFutureValue` 。 可选。 只读。|
|numberOfCloudPcStatusDeprovisioning|Int32|状态为 的云电脑数量 `deprovisioning` 。 可选。 只读。|
|numberOfCloudPcStatusFailed|Int32|状态为 的云电脑数量 `failed` 。 可选。 只读。|
|numberOfCloudPcStatusInGracePeriod|Int32|状态为 的云电脑数量 `inGracePeriod` 。 可选。 只读。|
|numberOfCloudPcStatusNotProvisioned|Int32|状态为 的云电脑数量 `notProvisioned` 。 可选。 只读。|
|numberOfCloudPcStatusProvisioned|Int32|状态为 的云电脑数量 `provisioned` 。 可选。 只读。|
|numberOfCloudPcStatusProvisioning|Int32|状态为 的云电脑数量 `provisioning` 。 可选。 只读。|
|numberOfCloudPcStatusUnknown|Int32|状态为 的云电脑数量 `unknown` 。 可选。 只读。|
|numberOfCloudPcStatusUpgrading|Int32|状态为 的云电脑数量 `upgrading` 。 可选。 只读。|
|tenantDisplayName|String|托管显示名称租户的租户。 可选。 只读。|
|totalCloudPcConnectionStatus|Int32|给定托管租户的云电脑连接状态总数。 可选。 只读。|
|totalCloudPcStatus|Int32|给定托管租户的云电脑总数量。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcOverview",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcOverview",
  "id": "String (identifier)",
  "tenantDisplayName": "String",
  "totalCloudPcStatus": "Integer",
  "numberOfCloudPcStatusNotProvisioned": "Integer",
  "numberOfCloudPcStatusProvisioning": "Integer",
  "numberOfCloudPcStatusProvisioned": "Integer",
  "numberOfCloudPcStatusUpgrading": "Integer",
  "numberOfCloudPcStatusInGracePeriod": "Integer",
  "numberOfCloudPcStatusDeprovisioning": "Integer",
  "numberOfCloudPcStatusFailed": "Integer",
  "numberOfCloudPcStatusUnknown": "Integer",
  "totalCloudPcConnectionStatus": "Integer",
  "numberOfCloudPcConnectionStatusPending": "Integer",
  "numberOfCloudPcConnectionStatusRunning": "Integer",
  "numberOfCloudPcConnectionStatusPassed": "Integer",
  "numberOfCloudPcConnectionStatusFailed": "Integer",
  "numberOfCloudPcConnectionStatusUnkownFutureValue": "Integer",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
