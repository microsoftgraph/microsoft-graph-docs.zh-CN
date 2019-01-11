---
title: mobileAppIntentAndState 资源类型
description: MobileApp 意图和给定的设备的安装状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 037faeb02f18f304153dbe19fef640cc1183ddcd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819794"
---
# <a name="mobileappintentandstate-resource-type"></a>mobileAppIntentAndState 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

MobileApp 意图和给定的设备的安装状态。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 mobileAppIntentAndStates](../api/intune-troubleshooting-mobileappintentandstate-list.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)集合|列出属性和[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象之间的关系。|
|[获取 mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|读取属性和[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象的关系。|
|[创建 mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|创建新的[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象。|
|[删除 mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|无|删除[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)。|
|[更新 mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|更新[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID|
|managedDeviceIdentifier|String|Intune 创建或收集的设备标识符。|
|userId|String|尝试注册设备的用户的标识符。|
|mobileAppList|[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)集合|负载方法和租户的状态的列表。|

## <a name="relationships"></a>Relationships
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





