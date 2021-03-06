---
title: deviceAppManagementTask 资源类型
description: 设备应用程序管理任务。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 51e8c7e057dc660e348dec17e8fa4e4704c7c202
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222518"
---
# <a name="deviceappmanagementtask-resource-type"></a>deviceAppManagementTask 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备应用程序管理任务。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceAppManagementTasks](../api/intune-partnerintegration-deviceappmanagementtask-list.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) 集合|列出 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) 对象的属性和关系。|
|[获取 deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-get.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|读取 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) 对象的属性和关系。|
|[创建 deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-create.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|创建新的 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) 对象。|
|[删除 deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-delete.md)|无|删除 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。|
|[更新 deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-update.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|更新 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) 对象的属性。|
|[updateStatus 操作](../api/intune-partnerintegration-deviceappmanagementtask-updatestatus.md)|无|设置任务的状态并附加注释。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体键。|
|displayName|String|名称。|
|description|String|说明。|
|createdDateTime|DateTimeOffset|创建日期。|
|dueDateTime|DateTimeOffset|到期日期。|
|“类别”|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|类别。 可取值为：`unknown`、`advancedThreatProtection`。|
|priority|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|优先级。 可取值为：`none`、`high`、`low`。|
|Creator|String|创建者的电子邮件地址。|
|creatorNotes|String|来自创建者的注释。|
|assignedTo|String|将此任务分配到的管理员的姓名或电子邮件。|
|status|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|状态。 可取值为：`unknown`、`pending`、`active`、`completed`、`rejected`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagementTask"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
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
  "status": "String"
}
```




