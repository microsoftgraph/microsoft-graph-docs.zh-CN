---
title: mobileAppIntentAndState 资源类型
description: MobileApp 意图和给定的设备的安装状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 01792d30bdf821d4dd0795926e116bdc12b95ad9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402403"
---
# <a name="mobileappintentandstate-resource-type"></a>mobileAppIntentAndState 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




