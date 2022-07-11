---
title: deviceCustomAttributeShellScript 资源类型
description: 表示 macOS 的自定义属性脚本。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 73f970193eb2386d98ad128660681efe70d287bc
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671302"
---
# <a name="devicecustomattributeshellscript-resource-type"></a>deviceCustomAttributeShellScript 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 macOS 的自定义属性脚本。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceCustomAttributeShellScripts](../api/intune-devices-devicecustomattributeshellscript-list.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) 集合|列出 [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) 对象的属性和关系。|
|[获取 deviceCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-get.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|读取 [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) 对象的属性和关系。|
|[创建 deviceCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-create.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|创建新的 [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) 对象。|
|[删除 deviceCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-delete.md)|None|删除 [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)。|
|[更新 deviceCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-update.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|更新 [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) 对象的属性。|
|[分配操作](../api/intune-devices-devicecustomattributeshellscript-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|自定义属性实体的唯一标识符。|
|customAttributeName|字符串|自定义属性的名称。|
|customAttributeType|[deviceCustomAttributeValueType](../resources/intune-devices-devicecustomattributevaluetype.md)|自定义属性值的预期类型。 可取值为：`integer`、`string`、`dateTime`。|
|displayName|字符串|设备管理脚本的名称。|
|说明|String|设备管理脚本的可选说明。|
|scriptContent|Binary|脚本内容。|
|createdDateTime|DateTimeOffset|创建设备管理脚本的日期和时间。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|上次修改设备管理脚本的日期和时间。 此属性是只读的。|
|runAsAccount|[runAsAccountType](../resources/intune-devices-runasaccounttype.md)|指示执行上下文的类型。 可取值为：`system`、`user`。|
|fileName|String|脚本文件名。|
|roleScopeTagIds|String collection|此 PowerShellScript 实例的范围标记 ID 列表。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) 集合|设备管理脚本的组分配列表。|
|assignments|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 集合|设备管理脚本的组分配列表。|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|运行设备管理脚本摘要。|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 集合|此脚本在所有设备中的运行状态列表。|
|userRunStates|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 集合|此脚本在所有用户中的运行状态列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCustomAttributeShellScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCustomAttributeShellScript",
  "id": "String (identifier)",
  "customAttributeName": "String",
  "customAttributeType": "String",
  "displayName": "String",
  "description": "String",
  "scriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```




