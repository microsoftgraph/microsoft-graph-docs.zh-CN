---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b1a49496357a3688bd9f484d8759fdd0c2140eb
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122628"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a>deviceOperatingSystemSummary 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备操作系统摘要。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|androidCount|Int32|Android 设备计数。|
|iosCount|Int32|iOS 设备计数。|
|macOSCount|Int32|Mac OS X 设备计数。|
|windowsMobileCount|Int32|Windows 移动设备计数。|
|windowsCount|Int32|Windows 设备计数。|
|unknownCount|Int32|未知设备计数。|
|androidDedicatedCount|Int32|专用 Android 设备的数量。|
|androidDeviceAdminCount|Int32|设备管理 Android 设备的数量。|
|androidFullyManagedCount|Int32|完全管理的 Android 设备的数量。|
|androidWorkProfileCount|Int32|工作配置文件 Android 设备的数量。|
|androidCorporateWorkProfileCount|Int32|企业工作配置文件 Android 设备的计数。 也称为企业拥有的个人启用 ("解决) 。 有效值-1 到2147483647|
|configMgrDeviceCount|Int32|ConfigMgr 托管设备的数量。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024,
  "androidDedicatedCount": 1024,
  "androidDeviceAdminCount": 1024,
  "androidFullyManagedCount": 1024,
  "androidWorkProfileCount": 1024,
  "androidCorporateWorkProfileCount": 1024,
  "configMgrDeviceCount": 1024
}
```



