---
title: userExperienceAnalyticsAutopilotDevicesSummary 资源类型
description: 未准备好 Windows Autopilot 的设备用户体验分析摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 27faa3cf52ba5b0118137b1d64c63552d9e4f127
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159369"
---
# <a name="userexperienceanalyticsautopilotdevicessummary-resource-type"></a>userExperienceAnalyticsAutopilotDevicesSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

未准备好 Windows Autopilot 的设备用户体验分析摘要。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|devicesNotAutopilotRegistered|Int32|未注册 autopilot 的 intune 设备计数。|
|devicesWithoutAutopilotProfileAssigned|Int32|未分配 autopilot 配置文件的 intune 设备计数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
  "devicesNotAutopilotRegistered": 1024,
  "devicesWithoutAutopilotProfileAssigned": 1024
}
```




