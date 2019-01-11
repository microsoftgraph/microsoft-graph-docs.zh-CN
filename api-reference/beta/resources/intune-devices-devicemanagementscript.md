---
title: deviceManagementScript 资源类型
description: Intune 将使客户能够在注册的 windows 10 Azure Active Directory 加入设备上运行其 Powershell 脚本。 一次或定期，可以运行该脚本。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 321d525aaf9de386ba639bc904915a06eda56a75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811044"
---
# <a name="devicemanagementscript-resource-type"></a>deviceManagementScript 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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
|id|字符串|设备管理脚本的唯一标识符。|
|displayName|字符串|设备管理脚本的名称。|
|说明|字符串|设备管理脚本的可选说明。|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|Script to run 时间间隔。 如果未定义脚本将运行一次|
|scriptContent|Binary|脚本内容。|
|createdDateTime|DateTimeOffset|创建设备管理脚本的日期和时间。|
|lastModifiedDateTime|DateTimeOffset|日期和设备管理脚本上次修改的时间。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示执行上下文中运行的设备管理脚本的类型。 可取值为：`system`、`user`。|
|enforceSignatureCheck|布尔|指示是否需要签脚本签名。|
|fileName|String|脚本文件的名称。|

## <a name="relationships"></a>Relationships
|关系|类型|Description|
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
  "fileName": "String"
}
```





