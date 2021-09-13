---
title: comanagedDevicesSummary 资源类型
description: 共同管理的设备的摘要数据
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aa734753a13777e93f8018ce0e13267a485044a7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137852"
---
# <a name="comanageddevicessummary-resource-type"></a>comanagedDevicesSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

共同管理的设备的摘要数据

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|inventoryCount|Int32|"清单"轻扫的设备数。 此属性是只读的。|
|compliancePolicyCount|Int32|具有 CompliancePolicy swung-over 的设备数。 此属性是只读的。|
|resourceAccessCount|Int32|ResourceAccess 轻扫的设备数。 此属性是只读的。|
|configurationSettingsCount|Int32|具有 ConfigurationSettings 轻扫的设备数。 此属性是只读的。|
|windowsUpdateForBusinessCount|Int32|WindowsUpdateForBusiness 轻扫的设备数。 此属性是只读的。|
|endpointProtectionCount|Int32|EndpointProtection 轻扫的设备数。 此属性是只读的。|
|modernAppsCount|Int32|使用 ModernApps 轻扫的设备数。 此属性是只读的。|
|officeAppsCount|Int32|具有 OfficeApps 轻扫的设备数。 此属性是只读的。|
|totalComanagedCount|Int32|设备Co-Managed数。 此属性是只读的。|

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



