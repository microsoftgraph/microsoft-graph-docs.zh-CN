---
title: deviceManagementScript 资源类型
description: Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本的功能。 脚本可以运行一次, 也可以定期运行。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19e61bf994a21305b4cf081c593b8d46cbb7806f
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572416"
---
# <a name="devicemanagementscript-resource-type"></a>deviceManagementScript 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本的功能。 脚本可以运行一次, 也可以定期运行。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementScripts](../api/intune-devices-devicemanagementscript-list.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)集合|列出[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性和关系。|
|[获取 deviceManagementScript](../api/intune-devices-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|读取[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性和关系。|
|[创建 deviceManagementScript](../api/intune-devices-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|创建新的[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象。|
|[删除 deviceManagementScript](../api/intune-devices-devicemanagementscript-delete.md)|None|删除[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)。|
|[更新 deviceManagementScript](../api/intune-devices-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|更新[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性。|
|[分配操作](../api/intune-devices-devicemanagementscript-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备管理脚本的唯一标识符。|
|displayName|字符串|设备管理脚本的名称。|
|说明|字符串|设备管理脚本的可选说明。|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|脚本运行的间隔。 如果未定义, 脚本将运行一次|
|scriptContent|二进制数|脚本内容。|
|createdDateTime|DateTimeOffset|设备管理脚本的创建日期和时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改设备管理脚本的日期和时间。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示执行上下文的类型。 可取值为：`system`、`user`。|
|enforceSignatureCheck|Boolean|指示是否需要检查脚本签名。|
|fileName|String|脚本文件名。|
|roleScopeTagIds|String collection|此 PowerShellScript 实例的范围标记 id 的列表。|
|runAs32Bit|Boolean|一个指示 PowerShell 脚本是否应作为32位运行的值|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合|设备管理脚本的组分配的列表。|
|assignments|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合|设备管理脚本的组分配的列表。|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|设备管理脚本的运行摘要。|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合|此脚本在所有设备上的运行状态列表。|
|userRunStates|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合|此脚本在所有用户中的运行状态列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
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
  "runAs32Bit": true
}
```




