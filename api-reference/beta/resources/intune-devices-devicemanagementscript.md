---
title: deviceManagementScript 资源类型
description: Intune 将使客户能够在注册的 windows 10 Azure Active Directory 加入设备上运行其 Powershell 脚本。 一次或定期，可以运行该脚本。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4fda826ec8033cd51ad4dd13dbc5b523a21e9e3a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412525"
---
# <a name="devicemanagementscript-resource-type"></a>deviceManagementScript 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Intune 将使客户能够在注册的 windows 10 Azure Active Directory 加入设备上运行其 Powershell 脚本。 一次或定期，可以运行该脚本。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 deviceManagementScripts](../api/intune-devices-devicemanagementscript-list.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)集合|列出属性和[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象之间的关系。|
|[获取 deviceManagementScript](../api/intune-devices-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|读取属性和[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的关系。|
|[创建 deviceManagementScript](../api/intune-devices-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|创建新的[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象。|
|[删除 deviceManagementScript](../api/intune-devices-devicemanagementscript-delete.md)|无|删除[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)。|
|[更新 deviceManagementScript](../api/intune-devices-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|更新[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性。|
|[assign 操作](../api/intune-devices-devicemanagementscript-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备管理脚本的唯一标识符。|
|displayName|String|设备管理脚本的名称。|
|说明|String|设备管理脚本的可选说明。|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|Script to run 时间间隔。 如果未定义脚本将运行一次|
|scriptContent|Binary|脚本内容。|
|createdDateTime|DateTimeOffset|创建设备管理脚本的日期和时间。|
|lastModifiedDateTime|DateTimeOffset|日期和设备管理脚本上次修改的时间。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示执行上下文中运行的设备管理脚本的类型。 可取值为：`system`、`user`。|
|enforceSignatureCheck|Boolean|指示是否需要签脚本签名。|
|fileName|String|脚本文件的名称。|
|roleScopeTagIds|String 集合|此 PowerShellScript 实例范围标记 Id 的列表。|
|runAs32Bit|Boolean|一个值，该值的 PowerShell 脚本是否应运行 32 位|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合|设备管理脚本的组分配列表。|
|assignments|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合|设备管理脚本的组分配列表。|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|运行设备管理脚本摘要。|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合|此脚本跨所有设备的运行状态的列表。|
|userRunStates|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合|列表的所有用户此脚本运行状态。|

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




