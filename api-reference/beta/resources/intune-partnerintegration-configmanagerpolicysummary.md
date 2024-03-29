---
title: configManagerPolicySummary 资源类型
description: ConfigManager 策略摘要。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 88c31f9314f7cc4c55c68b328768e3119d913298
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033453"
---
# <a name="configmanagerpolicysummary-resource-type"></a>configManagerPolicySummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ConfigManager 策略摘要。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|targetedDeviceCount|Int32|策略所面向的设备数量。|
|compliantDeviceCount|Int32|评估为符合策略的设备数量。|
|nonCompliantDeviceCount|Int32|策略评估为不相容的设备数量。|
|failedDeviceCount|Int32|策略未能评估的设备数。|
|pendingDeviceCount|Int32|已确认策略但正在等待评估的设备数量。|
|enforcedDeviceCount|Int32|策略已修正的设备数。|

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



