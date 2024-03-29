---
title: deviceManagementScript 资源类型
description: Intune使客户能够在已注册的 Windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本。 脚本可以运行一次或定期。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2fbb6e2bc1cdbd2e567f124228a7ed56315bde71
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441739"
---
# <a name="devicemanagementscript-resource-type"></a>deviceManagementScript 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Intune使客户能够在已注册的 Windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本。 脚本可以运行一次或定期。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementScripts](../api/intune-shared-devicemanagementscript-list.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 集合|列出 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象的属性和关系。|
|[获取 deviceManagementScript](../api/intune-shared-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|读取 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象的属性和关系。|
|[创建 deviceManagementScript](../api/intune-shared-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|创建新的 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象。|
|[删除 deviceManagementScript](../api/intune-shared-devicemanagementscript-delete.md)|无|删除 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)。|
|[更新 deviceManagementScript](../api/intune-shared-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|更新 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象的属性。|
|**设备管理**|
|[分配操作](../api/intune-shared-devicemanagementscript-assign.md)|无|尚未记录|
|**策略集**|
|[hasPayloadLinks 操作](../api/intune-shared-devicemanagementscript-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备管理脚本的唯一标识符。|
|displayName|String|设备管理脚本的名称。|
|description|String|设备管理脚本的可选说明。|
|scriptContent|Binary|脚本内容。|
|createdDateTime|DateTimeOffset|创建设备管理脚本的日期和时间。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|上次修改设备管理脚本的日期和时间。 此属性是只读的。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示执行上下文的类型。 可取值为：`system`、`user`。|
|enforceSignatureCheck|Boolean|指示是否需要检查脚本签名。|
|fileName|String|脚本文件名。|
|roleScopeTagIds|String collection|此 PowerShellScript 实例的范围标记 ID 列表。|
|runAs32Bit|Boolean|一个值，该值指示 PowerShell 脚本是否应以 32 位方式运行|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|**设备管理**|
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
  "@odata.type": "microsoft.graph.deviceManagementScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
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



