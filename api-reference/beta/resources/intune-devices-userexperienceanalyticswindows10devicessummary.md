---
title: userExperienceAnalyticsWindows10DevicesSummary 资源类型
description: 用户体验分析可随时随地使用 Windows 10 设备摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f43c2848902b6d9fbb3e54a2fd9a8ac36edc0793
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146757"
---
# <a name="userexperienceanalyticswindows10devicessummary-resource-type"></a>userExperienceAnalyticsWindows10DevicesSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析可随时随地使用 Windows 10 设备摘要。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|unsupportedOSversionDeviceCount|Int32|具有不受支持的操作系统版本的 Windows 10 设备计数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary",
  "unsupportedOSversionDeviceCount": 1024
}
```




