---
title: comanagedDevicesSummary 资源类型
description: Co 托管设备的摘要数据
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 42a92fd725c9f0b99037825c240dd017bf6c9c82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060774"
---
# <a name="comanageddevicessummary-resource-type"></a>comanagedDevicesSummary 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Co 托管设备的摘要数据

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|inventoryCount|Int32|具有库存 swung 的设备数量。 此属性是只读的。|
|compliancePolicyCount|Int32|具有 CompliancePolicy swung 的设备数量。 此属性是只读的。|
|resourceAccessCount|Int32|具有 ResourceAccess swung 的设备数量。 此属性是只读的。|
|configurationSettingsCount|Int32|具有 ConfigurationSettings swung 的设备数量。 此属性是只读的。|
|windowsUpdateForBusinessCount|Int32|具有 WindowsUpdateForBusiness swung 的设备数量。 此属性是只读的。|
|endpointProtectionCount|Int32|具有 EndpointProtection swung 的设备数量。 此属性是只读的。|
|modernAppsCount|Int32|具有 ModernApps swung 的设备数量。 此属性是只读的。|
|officeAppsCount|Int32|具有 Officeoffice swung 的设备数量。 此属性是只读的。|
|totalComanagedCount|Int32|共同管理的设备的数量。 此属性是只读的。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagedDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagedDevicesSummary",
  "inventoryCount": 1024,
  "compliancePolicyCount": 1024,
  "resourceAccessCount": 1024,
  "configurationSettingsCount": 1024,
  "windowsUpdateForBusinessCount": 1024,
  "endpointProtectionCount": 1024,
  "modernAppsCount": 1024,
  "officeAppsCount": 1024,
  "totalComanagedCount": 1024
}
```






