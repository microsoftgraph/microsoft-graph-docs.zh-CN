---
title: deviceHealthScript 资源类型
description: Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本的功能。 脚本可以运行一次，也可以定期运行。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6ad5fc4e12eeb28acbb6e4c0e0cbe085852feda3
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196957"
---
# <a name="devicehealthscript-resource-type"></a>deviceHealthScript 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本的功能。 脚本可以运行一次，也可以定期运行。


继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceHealthScripts](../api/intune-devices-devicehealthscript-list.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)集合|列出[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性和关系。|
|[获取 deviceHealthScript](../api/intune-devices-devicehealthscript-get.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|读取[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性和关系。|
|[创建 deviceHealthScript](../api/intune-devices-devicehealthscript-create.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|创建新的[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象。|
|[删除 deviceHealthScript](../api/intune-devices-devicehealthscript-delete.md)|无|删除[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)。|
|[更新 deviceHealthScript](../api/intune-devices-devicehealthscript-update.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|更新[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|设备管理脚本的唯一标识符。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|displayName|字符串|设备管理脚本的名称。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|说明|String|设备管理脚本的可选说明。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|脚本运行的间隔。 如果未定义，脚本将在从[DeviceManagementScript](../resources/intune-shared-devicemanagementscript.md)继承后运行。|
|scriptContent|Binary|脚本内容。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|createdDateTime|DateTimeOffset|设备管理脚本的创建日期和时间。 此属性是只读的。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改设备管理脚本的日期和时间。 此属性是只读的。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示执行上下文的类型。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)。 可取值为：`system`、`user`。|
|enforceSignatureCheck|Boolean|指示是否需要检查脚本签名。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|fileName|String|脚本文件名。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|roleScopeTagIds|String collection|此 PowerShellScript 实例的范围标记 Id 的列表。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|runAs32Bit|Boolean|一个指示 PowerShell 脚本是否应作为从[DeviceManagementScript](../resources/intune-shared-devicemanagementscript.md)继承的32位运行的值|
|complianceRule|[deviceHealthScriptComplianceRule](../resources/intune-devices-devicehealthscriptcompliancerule.md)|尚未记录|
|remediationScriptContent|Binary|尚未记录|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合|设备管理脚本的组分配的列表。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|assignments|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合|设备管理脚本的组分配的列表。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|设备管理脚本的运行摘要。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合|此脚本在所有设备上的运行状态列表。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|
|userRunStates|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合|此脚本在所有用户中的运行状态列表。 继承自[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "String",
    "operator": "String",
    "detectionValue": "String"
  },
  "remediationScriptContent": "binary"
}
```



