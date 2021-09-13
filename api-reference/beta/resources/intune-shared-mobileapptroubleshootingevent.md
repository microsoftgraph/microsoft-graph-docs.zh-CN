---
title: mobileAppTroubleshootingEvent 资源类型
description: 介绍支持多个工作流的 Microsoft Graph API 的 mobileAppTroubleshootingEvent 资源。
ms.localizationpriority: medium
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c4c522e6b6adf2a6a41c5e1a6a9e5b63fd64b9b0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020264"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a>mobileAppTroubleshootingEvent 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示设备管理和事件工作流疑难解答的用户设备应用程序安装状态的事件。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppTroubleshootingEvents](../api/intune-shared-mobileapptroubleshootingevent-list.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 集合|列出 [mobileAppTroubleshootingEvent 对象的属性和](../resources/intune-shared-mobileapptroubleshootingevent.md) 关系。|
|[获取 mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|读取 [mobileAppTroubleshootingEvent 对象的属性和](../resources/intune-shared-mobileapptroubleshootingevent.md) 关系。|
|[创建 mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|创建新的 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象。|
|[删除 mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|无|删除 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)。|
|[更新 mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|更新 [mobileAppTroubleshootingEvent 对象](../resources/intune-shared-mobileapptroubleshootingevent.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID。|
|**疑难解答**|
|additionalInformation|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|一组字符串键和字符串值对，提供有关疑难解答事件的其他信息 继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|applicationId|String|Intune 应用程序标识符。|
|correlationId|String|用于跟踪服务中的故障的 ID。 |
|eventDateTime|DateTimeOffset|事件发生的时间。 |
|eventName|String|与疑难解答事件对应的事件名称。 可选|
|history|[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) 集合|Intune 移动应用程序疑难解答历史记录项|
|managedDeviceIdentifier|String|Intune 创建或收集的设备标识符。|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|包含有关错误及其修正的详细信息的对象。 继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|userId|String|尝试注册设备的用户的标识符。|

## <a name="relationships"></a>关系
|关系|类型|描述|
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




