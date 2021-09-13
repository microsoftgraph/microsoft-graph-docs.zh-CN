---
title: deviceComplianceScript 资源类型
description: Intune 将为客户提供在已注册的 windows 10 (设备上) 运行其 Powershell 合规性脚本Azure Active Directory检测功能。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: adb65af1bc6c12a5b34b2b1c30b4959393dd4747
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057283"
---
# <a name="devicecompliancescript-resource-type"></a>deviceComplianceScript 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Intune 将为客户提供在已注册的 windows 10 (设备上) 运行其 Powershell 合规性脚本Azure Active Directory检测功能。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceComplianceScripts](../api/intune-devices-devicecompliancescript-list.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) 集合|列出 [deviceComplianceScript 对象的属性和](../resources/intune-devices-devicecompliancescript.md) 关系。|
|[获取 deviceComplianceScript](../api/intune-devices-devicecompliancescript-get.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|读取 [deviceComplianceScript 对象的属性和](../resources/intune-devices-devicecompliancescript.md) 关系。|
|[创建 deviceComplianceScript](../api/intune-devices-devicecompliancescript-create.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|创建新的 [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) 对象。|
|[删除 deviceComplianceScript](../api/intune-devices-devicecompliancescript-delete.md)|无|删除 [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)。|
|[更新 deviceComplianceScript](../api/intune-devices-devicecompliancescript-update.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|更新 [deviceComplianceScript 对象](../resources/intune-devices-devicecompliancescript.md) 的属性。|
|[分配操作](../api/intune-devices-devicecompliancescript-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备合规性脚本的唯一标识符|
|发布者|String|设备合规性脚本发布者的名称|
|version|String|设备合规性脚本的版本|
|displayName|String|设备合规性脚本的名称|
|说明|String|设备合规性脚本的说明|
|detectionScriptContent|二进制|检测 powershell 脚本的全部内容|
|createdDateTime|DateTimeOffset|创建设备合规性脚本的时间戳。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|修改设备合规性脚本的时间戳。 此属性是只读的。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示执行上下文的类型。 可取值为：`system`、`user`。|
|enforceSignatureCheck|Boolean|指示是否需要检查脚本签名|
|runAs32Bit|Boolean|指示 PowerShell 脚本 (脚本) 32 位运行|
|roleScopeTagIds|字符串集合|设备合规性脚本的范围标记标识列表|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 集合|设备合规性脚本的组分配列表|
|runSummary|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|设备合规性脚本的高级别运行摘要。|
|deviceRunStates|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 集合|跨所有设备的设备合规性脚本的运行状态列表|

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



