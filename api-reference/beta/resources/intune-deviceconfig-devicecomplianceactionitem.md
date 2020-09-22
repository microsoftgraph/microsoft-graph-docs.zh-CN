---
title: deviceComplianceActionItem 资源类型
description: 计划的操作配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 288337de04735026bc041ecbe9123bacb6daa90d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085120"
---
# <a name="devicecomplianceactionitem-resource-type"></a>deviceComplianceActionItem 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计划的操作配置

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceComplianceActionItems](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合|列出 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。|
|[获取 deviceComplianceActionItem](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|读取 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性和关系。|
|[创建 deviceComplianceActionItem](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|创建新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。|
|[删除 deviceComplianceActionItem](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|无|删除 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)。|
|[更新 deviceComplianceActionItem](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|更新 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
|gracePeriodHours|Int32|强制执行操作前要等待的小时数。 有效值为 0 至 8760|
|actionType|[deviceComplianceActionType](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|要执行的操作。 可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock`。|
|notificationTemplateId|String|要使用的通知消息模板|
|notificationMessageCCList|String collection|指定抄送此通知邮件的人员的组 ID 列表。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```






