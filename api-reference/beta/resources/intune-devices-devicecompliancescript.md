---
title: deviceComplianceScript 资源类型
description: Intune使客户能够在已注册的 Windows 10 Azure Active Directory 联接设备上运行其 Powershell 合规性脚本 (检测) 。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 04349bd414df14ca1359ea42523a197754b12622
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666877"
---
# <a name="devicecompliancescript-resource-type"></a>deviceComplianceScript 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Intune使客户能够在已注册的 Windows 10 Azure Active Directory 联接设备上运行其 Powershell 合规性脚本 (检测) 。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceComplianceScripts](../api/intune-devices-devicecompliancescript-list.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) 集合|列出 [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) 对象的属性和关系。|
|[获取 deviceComplianceScript](../api/intune-devices-devicecompliancescript-get.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|读取 [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) 对象的属性和关系。|
|[创建 deviceComplianceScript](../api/intune-devices-devicecompliancescript-create.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|创建新的 [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) 对象。|
|[删除 deviceComplianceScript](../api/intune-devices-devicecompliancescript-delete.md)|None|删除 [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)。|
|[更新 deviceComplianceScript](../api/intune-devices-devicecompliancescript-update.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|更新 [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) 对象的属性。|
|[分配操作](../api/intune-devices-devicecompliancescript-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备符合性脚本的唯一标识符|
|发布者|String|设备符合性脚本发布者名称|
|version|String|设备符合性脚本的版本|
|displayName|字符串|设备符合性脚本的名称|
|说明|String|设备符合性脚本的说明|
|detectionScriptContent|Binary|检测 powershell 脚本的整个内容|
|createdDateTime|DateTimeOffset|创建设备符合性脚本的时间戳。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|修改设备符合性脚本的时间戳。 此属性是只读的。|
|runAsAccount|[runAsAccountType](../resources/intune-devices-runasaccounttype.md)|指示执行上下文的类型。 可取值为：`system`、`user`。|
|enforceSignatureCheck|Boolean|指示是否需要检查脚本签名|
|runAs32Bit|布尔|指示 PowerShell 脚本 () 是否应以 32 位方式运行|
|roleScopeTagIds|String collection|设备符合性脚本的作用域标记 ID 列表|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 集合|设备符合性脚本的组分配列表|
|runSummary|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|设备符合性脚本的高级运行摘要。|
|deviceRunStates|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 集合|跨所有设备的设备符合性脚本的运行状态列表|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "id": "String (identifier)",
  "publisher": "String",
  "version": "String",
  "displayName": "String",
  "description": "String",
  "detectionScriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




