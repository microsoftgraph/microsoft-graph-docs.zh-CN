---
title: comanagementEligibleDevicesSummary 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03baadeea1441d5eecc1ff6e8974724b19a59949
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697782"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a>comanagementEligibleDevicesSummary 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|comanagedCount|Int32|已 Co-Managed 的设备计数|
|eligibleCount|Int32|完全符合条件的设备计数 Co-Management|
|eligibleButNotAzureAdJoinedCount|Int32|符合 Co-Management 但尚未加入 Azure Active Directory 的设备的计数|
|needsOsUpdateCount|Int32|在 OS 更新后符合 Co-Management 的设备的计数|
|ineligibleCount|Int32|不符合要求的设备的计数 Co-Management|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagementEligibleDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevicesSummary",
  "comanagedCount": 1024,
  "eligibleCount": 1024,
  "eligibleButNotAzureAdJoinedCount": 1024,
  "needsOsUpdateCount": 1024,
  "ineligibleCount": 1024
}
```





