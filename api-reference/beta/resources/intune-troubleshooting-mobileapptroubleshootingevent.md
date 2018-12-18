---
title: mobileAppTroubleshootingEvent 资源类型
description: 代表用户设备应用程序事件安装状态。
author: tfitzmac
ms.openlocfilehash: 92b16d0dd3678aed8cec810f27172e05f37f1ad8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314398"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a>mobileAppTroubleshootingEvent 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

代表用户设备应用程序事件安装状态。

继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 mobileAppTroubleshootingEvents](../api/intune-troubleshooting-mobileapptroubleshootingevent-list.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)集合|列出属性和[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)对象之间的关系。|
|[获取 mobileAppTroubleshootingEvent](../api/intune-troubleshooting-mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|读取属性和[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)对象的关系。|
|[创建 mobileAppTroubleshootingEvent](../api/intune-troubleshooting-mobileapptroubleshootingevent-create.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|创建新的[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)对象。|
|[删除 mobileAppTroubleshootingEvent](../api/intune-troubleshooting-mobileapptroubleshootingevent-delete.md)|无|删除[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)。|
|[更新 mobileAppTroubleshootingEvent](../api/intune-troubleshooting-mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|更新[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|eventDateTime|DateTimeOffset|事件发生的时间。 继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|correlationId|String|用于跟踪服务中的故障的 ID。 继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|managedDeviceIdentifier|String|Intune 创建或收集的设备标识符。|
|userId|String|尝试注册设备的用户的标识符。|
|applicationId|String|Intune 应用程序标识符。|
|历史记录|[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)集合|疑难解答历史记录项 Intune 移动应用程序|

## <a name="relationships"></a>Relationships
无
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





