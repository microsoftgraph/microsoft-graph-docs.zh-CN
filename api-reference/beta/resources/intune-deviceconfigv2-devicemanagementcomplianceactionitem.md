---
title: deviceManagementComplianceActionItem 资源类型
description: 计划的规则操作
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 097ab8a552e4675570fc85139924615f32b8fd0d
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697249"
---
# <a name="devicemanagementcomplianceactionitem-resource-type"></a>deviceManagementComplianceActionItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计划的规则操作

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementComplianceActionItems](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-list.md)|[deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md) 集合|列出 [deviceManagementComplianceActionItem 对象的属性和](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md) 关系。|
|[获取 deviceManagementComplianceActionItem](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-get.md)|[deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|读取 [deviceManagementComplianceActionItem 对象的属性和](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md) 关系。|
|[创建 deviceManagementComplianceActionItem](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-create.md)|[deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|创建新的 [deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md) 对象。|
|[删除 deviceManagementComplianceActionItem](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-delete.md)|无|删除 [deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)。|
|[更新 deviceManagementComplianceActionItem](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-update.md)|[deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|更新 [deviceManagementComplianceActionItem 对象](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|包含此设置的策略中的此设置的键。 自动生成。|
|gracePeriodHours|Int32|强制执行操作前要等待的小时数。 有效值为 0 至 8760|
|actionType|[deviceManagementComplianceActionType](../resources/intune-deviceconfigv2-devicemanagementcomplianceactiontype.md)|要采取的操作。 可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock`。|
|notificationTemplateId|String|要使用的通知消息模板|
|notificationMessageCCList|String collection|指定此通知邮件抄送对象的组 ID 列表。 此集合最多可包含 100 个元素。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```



