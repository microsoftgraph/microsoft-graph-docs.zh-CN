---
title: deviceShellScript 资源类型
description: Intune 将为客户提供在已注册的 Mac 操作系统设备上运行其 Shell 脚本的能力。 脚本可以运行一次或定期运行。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cc3553e5b2ca63f7d202b1cf197429815363780e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125825"
---
# <a name="deviceshellscript-resource-type"></a>deviceShellScript 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Intune 将为客户提供在已注册的 Mac 操作系统设备上运行其 Shell 脚本的能力。 脚本可以运行一次或定期运行。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceShellScripts](../api/intune-devices-deviceshellscript-list.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md) 集合|列出 [deviceShellScript 对象的属性和](../resources/intune-devices-deviceshellscript.md) 关系。|
|[获取 deviceShellScript](../api/intune-devices-deviceshellscript-get.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|读取 [deviceShellScript 对象的属性和](../resources/intune-devices-deviceshellscript.md) 关系。|
|[创建 deviceShellScript](../api/intune-devices-deviceshellscript-create.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|创建新的 [deviceShellScript](../resources/intune-devices-deviceshellscript.md) 对象。|
|[删除 deviceShellScript](../api/intune-devices-deviceshellscript-delete.md)|无|删除 [deviceShellScript](../resources/intune-devices-deviceshellscript.md)。|
|[更新 deviceShellScript](../api/intune-devices-deviceshellscript-update.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|更新 [deviceShellScript 对象](../resources/intune-devices-deviceshellscript.md) 的属性。|
|[分配操作](../api/intune-devices-deviceshellscript-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|executionFrequency|期限|脚本运行的间隔。 如果未定义，脚本将运行一次|
|retryCount|Int32|脚本失败时重试次数|
|blockExecutionNotifications|Boolean|不通知用户正在执行脚本|
|id|String|设备管理脚本的唯一标识符。|
|displayName|String|设备管理脚本的名称。|
|说明|String|设备管理脚本的可选说明。|
|scriptContent|二进制|脚本内容。|
|createdDateTime|DateTimeOffset|创建设备管理脚本的日期和时间。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|上次修改设备管理脚本的日期和时间。 此属性是只读的。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示执行上下文的类型。 可取值为：`system`、`user`。|
|fileName|String|脚本文件名。|
|roleScopeTagIds|字符串集合|此 PowerShellScript 实例的范围标记标识列表。|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|groupAssignments|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) 集合|设备管理脚本的组分配列表。|
|assignments|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 集合|设备管理脚本的组分配列表。|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|运行设备管理脚本摘要。|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 集合|此脚本在所有设备的运行状态列表。|
|userRunStates|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 集合|所有用户中此脚本的运行状态列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceShellScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "String (duration)",
  "retryCount": 1024,
  "blockExecutionNotifications": true,
  "id": "String (identifier)",
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



