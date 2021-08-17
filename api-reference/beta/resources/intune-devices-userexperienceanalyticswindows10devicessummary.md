---
title: userExperienceAnalyticsWindows10DevicesSummary 资源类型
description: 用户体验分析从任意位置到设备Windows 10工作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b8fdbb23b5b1d645423fa6c89267154a5b8c3cc903c7d914619d77373dea2049
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206282"
---
# <a name="userexperienceanalyticswindows10devicessummary-resource-type"></a>userExperienceAnalyticsWindows10DevicesSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析从任意位置到设备Windows 10工作。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|unsupportedOSversionDeviceCount|Int32|操作系统版本Windows 10的设备数量。|

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




