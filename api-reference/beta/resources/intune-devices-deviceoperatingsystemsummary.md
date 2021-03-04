---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de94b00a1660dc874e457d20315df2f3b0690164
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444481"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a>deviceOperatingSystemSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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
|androidDeviceAdminCount|Int32|设备管理员 Android 设备的数量。|
|androidFullyManagedCount|Int32|完全托管的 Android 设备的数量。|
|androidWorkProfileCount|Int32|Android 设备的工作配置文件数量。|
|androidCorporateWorkProfileCount|Int32|企业工作配置文件 Android 设备计数。 也称为公司拥有的个人启用 (的) 。 有效值 -1 到 2147483647|
|configMgrDeviceCount|Int32|ConfigMgr 托管设备的数量。|
|aospUserlessCount|Int32|无用户 AOSP Android 设备的数量。 有效值为 0 到 2147483647|
|aospUserAssociatedCount|Int32|AOSP 用户关联的 Android 设备的数量。 有效值为 0 到 2147483647|
|linuxCount|Int32|Linux OS 设备的数量。 有效值为 0 到 2147483647|

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
  "configMgrDeviceCount": 1024,
  "aospUserlessCount": 1024,
  "aospUserAssociatedCount": 1024,
  "linuxCount": 1024
}
```




