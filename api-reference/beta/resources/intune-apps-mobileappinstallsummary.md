---
title: mobileAppInstallSummary 资源类型
description: 包含移动应用的安装摘要的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d92ba2afe56607490c4bdf8b1d0443eb500be912
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817416"
---
# <a name="mobileappinstallsummary-resource-type"></a>mobileAppInstallSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含移动应用的安装摘要的属性。

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[获取 mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|读取 [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) 对象的属性和关系。|
|[更新 mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|更新 [mobileAppInstallSummary 对象](../resources/intune-apps-mobileappinstallsummary.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|installedDeviceCount|Int32|已成功安装此应用的设备数。|
|failedDeviceCount|Int32|未能安装此应用的设备数。|
|notApplicableDeviceCount|Int32|不适用于此应用的设备数。|
|notInstalledDeviceCount|Int32|未安装此应用的设备数。|
|pendingInstallDeviceCount|Int32|已通知安装此应用的设备数。|
|installedUserCount|Int32|其设备全部成功安装此应用的用户数。|
|failedUserCount|Int32|拥有 1 台或多台设备未能安装此应用的用户数量。|
|notApplicableUserCount|Int32|其设备均不适用于此应用的用户数。|
|notInstalledUserCount|Int32|具有 1 台或多台设备未安装此应用的用户数量。|
|pendingInstallUserCount|Int32|拥有 1 台或多台设备且已收到通知安装此应用且设备有 0 台失败的用户数量。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "pendingInstallDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notApplicableUserCount": 1024,
  "notInstalledUserCount": 1024,
  "pendingInstallUserCount": 1024
}
```



