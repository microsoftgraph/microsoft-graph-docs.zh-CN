---
title: mobileAppTroubleshootingEvent 资源类型
description: 介绍支持多个工作流的 Microsoft 图形 API for Intune 的 mobileAppTroubleshootingEvent 资源。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e13418289387784519a33478975dad15bc2b1e5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445081"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a>mobileAppTroubleshootingEvent 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示用于设备管理和事件工作流故障排除的用户设备应用程序安装状态的事件。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppTroubleshootingEvents](../api/intune-shared-mobileapptroubleshootingevent-list.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 集合|列出 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象的属性和关系。|
|[获取 mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|读取 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象的属性和关系。|
|[创建 mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|创建新的 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象。|
|[删除 mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|无|删除 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)。|
|[更新 mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|更新 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID。|
|**疑难解答**|
|additionalInformation|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|一组字符串键和字符串值对，提供有关从 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 继承的故障排除事件的其他信息|
|applicationId|String|Intune应用程序标识符。|
|correlationId|String|用于跟踪服务中的故障的 ID。 |
|eventDateTime|DateTimeOffset|事件发生的时间。 |
|eventName|String|与故障排除事件对应的事件名称。 可选|
|历史|[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) 集合|Intune移动应用程序故障排除历史记录项|
|managedDeviceIdentifier|String|Intune 创建或收集的设备标识符。|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|包含有关错误及其修正的详细信息的对象。 继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|userId|String|尝试注册设备的用户的标识符。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|**设备管理**|
|appLogCollectionRequests|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) 集合|AppLogUploadRequest 的集合属性。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
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
  ],
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "applicationId": "String",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "String (timestamp)"
    }
  ]
}
```




