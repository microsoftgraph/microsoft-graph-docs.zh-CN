---
title: mobileAppIntentAndStateDetail 资源类型
description: 给定设备的移动应用意图和安装状态。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 92f3e301e16b14f7a1aac1ed9dc27a60d53b2850
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59100888"
---
# <a name="mobileappintentandstatedetail-resource-type"></a>mobileAppIntentAndStateDetail 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定设备的移动应用意图和安装状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|applicationId|String|MobieApp 标识符。|
|displayName|String|管理员提供或导入的应用标题。|
|mobileAppIntent|[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md)|移动应用意图。 可取值为：`available`、`notAvailable`、`requiredInstall`、`requiredUninstall`、`requiredAndAvailableInstall`、`availableInstallWithoutEnrollment` 或 `exclude`。|
|displayVersion|String|应用程序的可读人工版本|
|installState|[resultantAppState](../resources/intune-troubleshooting-resultantappstate.md)|应用的安装状态。 可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。|
|supportedDeviceTypes|[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) 集合|应用支持的平台。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndStateDetail",
  "applicationId": "String",
  "displayName": "String",
  "mobileAppIntent": "String",
  "displayVersion": "String",
  "installState": "String",
  "supportedDeviceTypes": [
    {
      "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
      "type": "String",
      "minimumOperatingSystemVersion": "String",
      "maximumOperatingSystemVersion": "String"
    }
  ]
}
```




