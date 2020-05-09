---
title: deviceHealthScriptAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ba8735cbe386d32e9f54e05c500a0bd5b3413e6
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44175558"
---
# <a name="devicehealthscriptassignment-resource-type"></a>deviceHealthScriptAssignment 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于将设备管理脚本分配给组的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceHealthScriptAssignments](../api/intune-devices-devicehealthscriptassignment-list.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)集合|列出[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象的属性和关系。|
|[获取 deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-get.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|读取[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象的属性和关系。|
|[创建 deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-create.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|创建新的[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象。|
|[删除 deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-delete.md)|无|删除[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)。|
|[更新 deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-update.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|更新[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|设备运行状况脚本分配实体的键。 此属性是只读的。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|将脚本设定为的 Azure Active Directory 组|
|runRemediationScript|Boolean|确定是只运行检测脚本还是运行两个检测脚本和修正脚本|
|runSchedule|[deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|目标组的脚本运行计划|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  },
  "runRemediationScript": true,
  "runSchedule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule",
    "interval": 1024,
    "useUtc": true,
    "time": "String (time of day)"
  }
}
```



