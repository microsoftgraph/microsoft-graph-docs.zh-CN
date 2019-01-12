---
title: deviceComplianceActionItem 资源类型
description: 计划的操作配置
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0676acc44946b327772083ccd6e46e3f47df648f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980193"
---
# <a name="devicecomplianceactionitem-resource-type"></a>deviceComplianceActionItem 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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
|id|String|实体的键。|
|gracePeriodHours|Int32|强制执行操作前要等待的小时数。 有效值为 0 至 8760|
|actionType|[deviceComplianceActionType](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|要采取什么操作。 可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock`。|
|notificationTemplateId|String|要使用的通知消息模板|
|notificationMessageCCList|String 集合|指定抄送此通知邮件的人员的组 ID 列表。|

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





