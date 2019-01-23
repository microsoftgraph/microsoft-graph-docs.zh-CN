---
title: deviceManagementTroubleshootingEvent 资源类型
description: 表示一般性故障的事件。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a9c550b1f1285d86602aea1c8d9328869123a18f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413666"
---
# <a name="devicemanagementtroubleshootingevent-resource-type"></a>deviceManagementTroubleshootingEvent 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示一般性故障的事件。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementTroubleshootingEvents](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-list.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 集合|列出 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性和关系。|
|[获取 deviceManagementTroubleshootingEvent](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-get.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|读取 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性和关系。|
|[创建 deviceManagementTroubleshootingEvent](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-create.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|创建新的 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。|
|[删除 deviceManagementTroubleshootingEvent](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-delete.md)|无|删除 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)。|
|[更新 deviceManagementTroubleshootingEvent](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-update.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|更新 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID|
|eventDateTime|DateTimeOffset|事件发生的时间。|
|correlationId|String|用于跟踪服务中的故障的 ID。|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|对象包含有关错误和其修复的详细的信息。|
|事件名称|String|对应于疑难解答事件的事件名称。 它是一个可选字段|
|additionalInformation|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|一组字符串键和字符串值对提供了有关疑难解答事件其他信息|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```




