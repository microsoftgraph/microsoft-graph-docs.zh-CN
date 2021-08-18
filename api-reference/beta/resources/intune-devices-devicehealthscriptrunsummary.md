---
title: deviceHealthScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d1bf94f10b164e13600989b6fed982f6426a505a9f952ff67a1aa97dc4843da5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54156196"
---
# <a name="devicehealthscriptrunsummary-resource-type"></a>deviceHealthScriptRunSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含设备管理脚本的运行摘要的属性。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceHealthScriptRunSummary](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|读取 [deviceHealthScriptRunSummary 对象的属性和](../resources/intune-devices-devicehealthscriptrunsummary.md) 关系。|
|[更新 deviceHealthScriptRunSummary](../api/intune-devices-devicehealthscriptrunsummary-update.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|更新 [deviceHealthScriptRunSummary 对象](../resources/intune-devices-devicehealthscriptrunsummary.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备运行状况脚本运行摘要实体的键。 此属性是只读的。|
|noIssueDetectedDeviceCount|Int32|检测脚本未发现问题且设备正常运行的设备数量|
|issueDetectedDeviceCount|Int32|检测脚本发现问题的设备数量|
|detectionScriptErrorDeviceCount|Int32|检测脚本执行遇到错误且未完成的设备数量|
|detectionScriptPendingDeviceCount|Int32|尚未运行最新版本的设备运行状况脚本的设备数量|
|detectionScriptNotApplicableDeviceCount|Int32|检测脚本不适用的设备数量|
|issueRemediatedDeviceCount|Int32|修正脚本能够解决检测到的问题的设备数量|
|remediationSkippedDeviceCount|Int32|已跳过修正的设备数|
|issueReoccurredDeviceCount|Int32|修复脚本成功执行但未能解决检测到的问题的设备数量|
|remediationScriptErrorDeviceCount|Int32|修正脚本执行遇到错误且未完成的设备数量|
|lastScriptRunDateTime|DateTimeOffset|脚本跨所有设备的上次运行时间|
|issueRemediatedCumulativeDeviceCount|Int32|过去 30 天内修正的设备数|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "detectionScriptNotApplicableDeviceCount": 1024,
  "issueRemediatedDeviceCount": 1024,
  "remediationSkippedDeviceCount": 1024,
  "issueReoccurredDeviceCount": 1024,
  "remediationScriptErrorDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": 1024
}
```




