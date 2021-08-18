---
title: deviceAppManagementTask 资源类型
description: 设备应用管理任务。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c539c1c2ee284641e7f63f0113ebc35f5ea866f3087339cf436f5f783c830be2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164165"
---
# <a name="deviceappmanagementtask-resource-type"></a>deviceAppManagementTask 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备应用管理任务。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceAppManagementTasks](../api/intune-partnerintegration-deviceappmanagementtask-list.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) 集合|列出 [deviceAppManagementTask 对象的属性和](../resources/intune-partnerintegration-deviceappmanagementtask.md) 关系。|
|[获取 deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-get.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|读取 [deviceAppManagementTask 对象的属性和](../resources/intune-partnerintegration-deviceappmanagementtask.md) 关系。|
|[创建 deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-create.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|创建新的 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) 对象。|
|[删除 deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-delete.md)|无|删除 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。|
|[更新 deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-update.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|更新 [deviceAppManagementTask 对象](../resources/intune-partnerintegration-deviceappmanagementtask.md) 的属性。|
|[updateStatus 操作](../api/intune-partnerintegration-deviceappmanagementtask-updatestatus.md)|无|设置任务的状态并附加注释。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体键。|
|displayName|字符串|名称。|
|description|String|说明。|
|createdDateTime|DateTimeOffset|创建日期。|
|dueDateTime|DateTimeOffset|截止日期。|
|“类别”|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|类别。 可取值为：`unknown`、`advancedThreatProtection`。|
|priority|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|优先级。 可取值为：`none`、`high`、`low`。|
|Creator|字符串|创建者的电子邮件地址。|
|creatorNotes|String|创建者的备注。|
|assignedTo|String|分配此任务的管理员的姓名或电子邮件。|
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




