---
title: mobileAppInstallSummary 资源类型
description: 包含的移动应用程序安装摘要属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2bd7c30c1b00e83731766bcd80f9a9fafd8e8b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416711"
---
# <a name="mobileappinstallsummary-resource-type"></a>mobileAppInstallSummary 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含的移动应用程序安装摘要属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|读取属性和[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的关系。|
|[更新 mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|更新[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|installedDeviceCount|Int32|已成功安装此应用程序的设备数。|
|failedDeviceCount|Int32|未能安装此应用程序的设备数。|
|notApplicableDeviceCount|Int32|不适用于此应用程序的设备数。|
|notInstalledDeviceCount|Int32|没有安装该应用程序的设备数目。|
|pendingInstallDeviceCount|Int32|已被通知安装此应用程序的设备数。|
|installedUserCount|Int32|所有成功安装此应用程序的设备的用户数。|
|failedUserCount|Int32|用户具有 1 或无法安装此应用程序的更多设备数。|
|notApplicableUserCount|Int32|其设备未所有适用于此应用程序的用户数。|
|notInstalledUserCount|Int32|未安装该应用程序的一个或多个设备的用户数。|
|pendingInstallUserCount|Int32|用户具有 1 或更多已经通知安装此应用程序和失败的 0 设备的设备数。|

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




