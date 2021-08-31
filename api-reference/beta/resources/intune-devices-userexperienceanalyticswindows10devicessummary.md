---
title: userExperienceAnalyticsWindows10DevicesSummary 资源类型
description: 用户体验分析从任意位置到设备Windows 10工作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: beeded0dfecec5f8c596e22a20c2352679a9fadc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797491"
---
# <a name="userexperienceanalyticswindows10devicessummary-resource-type"></a>userExperienceAnalyticsWindows10DevicesSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析从任意位置到设备Windows 10工作。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|unsupportedOSversionDeviceCount|Int32|操作系统Windows 10不支持的设备数。|

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



