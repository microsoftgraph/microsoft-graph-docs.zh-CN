---
title: deviceManagementComplianceScheduledActionForRule 资源类型
description: 计划的规则操作
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed7521f62566cb25a74ba3d4bacd46573edc8d79
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697248"
---
# <a name="devicemanagementcompliancescheduledactionforrule-resource-type"></a>deviceManagementComplianceScheduledActionForRule 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计划的规则操作

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementComplianceScheduledActionForRules](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-list.md)|[deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md) 集合|列出 [deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md) 对象的属性和关系。|
|[获取 deviceManagementComplianceScheduledActionForRule](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-get.md)|[deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|读取 [deviceManagementComplianceScheduledActionForRule 对象的属性和](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md) 关系。|
|[创建 deviceManagementComplianceScheduledActionForRule](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-create.md)|[deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|创建新的 [deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md) 对象。|
|[删除 deviceManagementComplianceScheduledActionForRule](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-delete.md)|无|删除 [deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)。|
|[更新 deviceManagementComplianceScheduledActionForRule](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-update.md)|[deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|更新 [deviceManagementComplianceScheduledActionForRule 对象](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|包含此设置的策略中的此设置的键。 自动生成。|
|ruleName|String|此计划操作适用的规则名称。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|scheduledActionConfigurations|[deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md) 集合|此合规性策略的计划操作配置列表。 此集合最多可包含 100 个元素。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementComplianceScheduledActionForRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementComplianceScheduledActionForRule",
  "id": "String (identifier)",
  "ruleName": "String"
}
```



