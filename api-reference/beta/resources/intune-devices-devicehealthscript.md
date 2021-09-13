---
title: deviceHealthScript 资源类型
description: Intune 将为客户提供在已注册的 windows 10 (设备上运行其 Powershell 运行状况脚本) 修正 + 检测Azure Active Directory功能。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8cd3dfe2a8a3dfbd775c655757728a62ff1f7759
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017399"
---
# <a name="devicehealthscript-resource-type"></a>deviceHealthScript 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Intune 将为客户提供在已注册的 windows 10 (设备上运行其 Powershell 运行状况脚本) 修正 + 检测Azure Active Directory功能。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceHealthScripts](../api/intune-devices-devicehealthscript-list.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md) 集合|列出 [deviceHealthScript 对象的属性和](../resources/intune-devices-devicehealthscript.md) 关系。|
|[获取 deviceHealthScript](../api/intune-devices-devicehealthscript-get.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|读取 [deviceHealthScript 对象的属性和](../resources/intune-devices-devicehealthscript.md) 关系。|
|[创建 deviceHealthScript](../api/intune-devices-devicehealthscript-create.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|创建新的 [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) 对象。|
|[删除 deviceHealthScript](../api/intune-devices-devicehealthscript-delete.md)|None|删除 [deviceHealthScript](../resources/intune-devices-devicehealthscript.md)。|
|[更新 deviceHealthScript](../api/intune-devices-devicehealthscript-update.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|更新 [deviceHealthScript 对象](../resources/intune-devices-devicehealthscript.md) 的属性。|
|[分配操作](../api/intune-devices-devicehealthscript-assign.md)|无|尚未记录|
|[updateGlobalScript 操作](../api/intune-devices-devicehealthscript-updateglobalscript.md)|String|更新专有设备运行状况脚本|
|[getGlobalScriptHighestAvailableVersion 操作](../api/intune-devices-devicehealthscript-getglobalscripthighestavailableversion.md)|String|更新专有设备运行状况脚本|
|[enableGlobalScripts 操作](../api/intune-devices-devicehealthscript-enableglobalscripts.md)|无|尚未记录|
|[areGlobalScriptsAvailable 函数](../api/intune-devices-devicehealthscript-areglobalscriptsavailable.md)|[globalDeviceHealthScriptState](../resources/intune-devices-globaldevicehealthscriptstate.md)|尚未记录|
|[getRemediationSummary 函数](../api/intune-devices-devicehealthscript-getremediationsummary.md)|[deviceHealthScriptRemediationSummary](../resources/intune-devices-devicehealthscriptremediationsummary.md)|尚未记录|
|[getRemediationHistory 函数](../api/intune-devices-devicehealthscript-getremediationhistory.md)|[deviceHealthScriptRemediationHistory](../resources/intune-devices-devicehealthscriptremediationhistory.md)|用于获取设备运行状况脚本修正数量的函数|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备运行状况脚本的唯一标识符|
|发布者|String|设备运行状况脚本发布者的名称|
|version|String|设备运行状况脚本的版本|
|displayName|String|设备运行状况脚本的名称|
|说明|String|设备运行状况脚本的说明|
|detectionScriptContent|二进制|检测 powershell 脚本的全部内容|
|remediationScriptContent|二进制|修正 powershell 脚本的全部内容|
|createdDateTime|DateTimeOffset|创建设备运行状况脚本的时间戳。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|修改设备运行状况脚本的时间戳。 此属性是只读的。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示执行上下文的类型。 可取值为：`system`、`user`。|
|enforceSignatureCheck|Boolean|指示是否需要检查脚本签名|
|runAs32Bit|Boolean|指示 PowerShell 脚本 (脚本) 32 位运行|
|roleScopeTagIds|String collection|设备运行状况脚本的范围标记标识列表|
|isGlobalScript|布尔值|确定这是否为 Microsoft 专有脚本。 专有脚本是只读的|
|highestAvailableVersion|String|Microsoft 专有脚本的最高可用版本|
|detectionScriptParameters|[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) 集合|ComplexType DetectionScriptParameters 对象的列表。|
|remediationScriptParameters|[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) 集合|ComplexType RemediationScriptParameters 对象的列表。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 集合|设备运行状况脚本的组分配列表|
|runSummary|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|设备运行状况脚本的高级别运行摘要。|
|deviceRunStates|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 集合|跨所有设备的设备运行状况脚本的运行状态列表|

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
  "publisher": "String",
  "version": "String",
  "displayName": "String",
  "description": "String",
  "detectionScriptContent": "binary",
  "remediationScriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "String"
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "String",
  "detectionScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "String",
      "description": "String",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "String"
    }
  ],
  "remediationScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "String",
      "description": "String",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "String"
    }
  ]
}
```



