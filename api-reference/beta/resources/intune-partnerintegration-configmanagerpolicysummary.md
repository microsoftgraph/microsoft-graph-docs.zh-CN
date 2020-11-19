---
title: configManagerPolicySummary 资源类型
description: ConfigManager 策略摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c63e85448b70abc76f4df0021c4f5516e778ebe0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301536"
---
# <a name="configmanagerpolicysummary-resource-type"></a>configManagerPolicySummary 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ConfigManager 策略摘要。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|targetedDeviceCount|Int32|策略的目标设备的数量。|
|compliantDeviceCount|Int32|评估为符合策略的设备数。|
|nonCompliantDeviceCount|Int32|评估为不符合策略的设备数量。|
|failedDeviceCount|Int32|该策略无法评估的设备数量。|
|pendingDeviceCount|Int32|已确认策略但正在等待评估的设备数量。|
|enforcedDeviceCount|Int32|已由策略修正的设备数量。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configManagerPolicySummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configManagerPolicySummary",
  "targetedDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "enforcedDeviceCount": 1024
}
```




