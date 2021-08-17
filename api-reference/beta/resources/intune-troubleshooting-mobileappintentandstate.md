---
title: mobileAppIntentAndState 资源类型
description: 给定设备的 MobileApp 意图和安装状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d8e5b3c8eb1e221adffcd79f65884c688067d1ba
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58255938"
---
# <a name="mobileappintentandstate-resource-type"></a>mobileAppIntentAndState 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定设备的 MobileApp 意图和安装状态。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppIntentAndStates](../api/intune-troubleshooting-mobileappintentandstate-list.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) 集合|列出 [mobileAppIntentAndState 对象的属性和](../resources/intune-troubleshooting-mobileappintentandstate.md) 关系。|
|[获取 mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|读取 [mobileAppIntentAndState 对象的属性和](../resources/intune-troubleshooting-mobileappintentandstate.md) 关系。|
|[创建 mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|创建新的 [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) 对象。|
|[删除 mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|无|删除 [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)。|
|[更新 mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|更新 [mobileAppIntentAndState 对象](../resources/intune-troubleshooting-mobileappintentandstate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID|
|managedDeviceIdentifier|String|Intune 创建或收集的设备标识符。|
|userId|字符串|尝试注册设备的用户的标识符。|
|mobileAppList|[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) 集合|租户的有效负载意图和状态列表。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppIntentAndState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "String (identifier)",
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
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
  ]
}
```




