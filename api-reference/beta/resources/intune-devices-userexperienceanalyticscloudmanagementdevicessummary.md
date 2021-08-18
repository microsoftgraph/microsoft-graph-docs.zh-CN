---
title: userExperienceAnalyticsCloudManagementDevicesSummary 资源类型
description: 用户体验从任意位置云管理设备摘要工作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d84f0e524f88025caf6ef116b08cec5d221dfac0e904e2a9c12eb85cd15dc3cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145304"
---
# <a name="userexperienceanalyticscloudmanagementdevicessummary-resource-type"></a>userExperienceAnalyticsCloudManagementDevicesSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验从任意位置云管理设备摘要工作。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|coManagedDeviceCount|Int32|共同管理的设备的总数。|
|intuneDeviceCount|Int32|未注册 autopilot 的 intune 设备计数。|
|tenantAttachDeviceCount|Int32|租户附加设备总数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary",
  "coManagedDeviceCount": 1024,
  "intuneDeviceCount": 1024,
  "tenantAttachDeviceCount": 1024
}
```




