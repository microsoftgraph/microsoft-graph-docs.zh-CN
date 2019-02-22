---
title: deviceComplianceScheduledActionForRule 资源类型
description: 计划的规则操作
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e201e66765c7a50fa372f33bea536c6c694c3fe2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165504"
---
# <a name="devicecompliancescheduledactionforrule-resource-type"></a>deviceComplianceScheduledActionForRule 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计划的规则操作

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceComplianceScheduledActionForRules](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-list.md)|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合|列出 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性和关系。|
|[获取 deviceComplianceScheduledActionForRule](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-get.md)|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|读取 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性和关系。|
|[创建 deviceComplianceScheduledActionForRule](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-create.md)|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|创建新的 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象。|
|[删除 deviceComplianceScheduledActionForRule](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-delete.md)|无|删除 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)。|
|[更新 deviceComplianceScheduledActionForRule](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-update.md)|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|更新 [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
|ruleName|String|此计划操作适用的规则名称。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|scheduledActionConfigurations|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 集合|此合规性策略的计划操作配置列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScheduledActionForRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "String (identifier)",
  "ruleName": "String"
}
```




