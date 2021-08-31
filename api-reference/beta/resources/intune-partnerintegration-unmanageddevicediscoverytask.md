---
title: unmanagedDeviceDiscoveryTask 资源类型
description: 此任务派生类型表示网络中发现非托管设备的列表。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f80d0cd1941334325721e3a08ec4d302a8c75c9c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58795155"
---
# <a name="unmanageddevicediscoverytask-resource-type"></a>unmanagedDeviceDiscoveryTask 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

此任务派生类型表示网络中发现非托管设备的列表。


继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unmanagedDeviceDiscoveryTasks](../api/intune-partnerintegration-unmanageddevicediscoverytask-list.md)|[unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) 集合|列出 [unmanagedDeviceDiscoveryTask 对象的属性和](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) 关系。|
|[获取 unmanagedDeviceDiscoveryTask](../api/intune-partnerintegration-unmanageddevicediscoverytask-get.md)|[unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|读取 [unmanagedDeviceDiscoveryTask 对象的属性和](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) 关系。|
|[创建 unmanagedDeviceDiscoveryTask](../api/intune-partnerintegration-unmanageddevicediscoverytask-create.md)|[unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|创建新的 [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) 对象。|
|[删除 unmanagedDeviceDiscoveryTask](../api/intune-partnerintegration-unmanageddevicediscoverytask-delete.md)|无|删除 [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)。|
|[更新 unmanagedDeviceDiscoveryTask](../api/intune-partnerintegration-unmanageddevicediscoverytask-update.md)|[unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|更新 [unmanagedDeviceDiscoveryTask 对象](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体键。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|displayName|String|名称。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|description|字符串|说明。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|createdDateTime|DateTimeOffset|创建日期。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|dueDateTime|DateTimeOffset|截止日期。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|“类别”|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|类别。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。 可取值为：`unknown`、`advancedThreatProtection`。|
|priority|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|优先级。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。 可取值为：`none`、`high`、`low`。|
|Creator|String|创建者的电子邮件地址。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|creatorNotes|String|创建者的备注。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|assignedTo|String|分配此任务的管理员的姓名或电子邮件。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|状态|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|状态。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。 可取值为：`unknown`、`pending`、`active`、`completed`、`rejected`。|
|unmanagedDevices|[unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md) 集合|在网络中发现的非托管设备。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unmanagedDeviceDiscoveryTask"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unmanagedDeviceDiscoveryTask",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "category": "String",
  "priority": "String",
  "creator": "String",
  "creatorNotes": "String",
  "assignedTo": "String",
  "status": "String",
  "unmanagedDevices": [
    {
      "@odata.type": "microsoft.graph.unmanagedDevice",
      "os": "String",
      "osVersion": "String",
      "ipAddress": "String",
      "deviceName": "String",
      "macAddress": "String",
      "domain": "String",
      "manufacturer": "String",
      "model": "String",
      "location": "String",
      "lastLoggedOnUser": "String",
      "lastSeenDateTime": "String (timestamp)"
    }
  ]
}
```



