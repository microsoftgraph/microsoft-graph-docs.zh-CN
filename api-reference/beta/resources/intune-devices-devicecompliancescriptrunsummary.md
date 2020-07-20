---
title: deviceComplianceScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c436261961be8938e8905bc9f19be1690c7f79c4
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789337"
---
# <a name="devicecompliancescriptrunsummary-resource-type"></a>deviceComplianceScriptRunSummary 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含设备管理脚本的运行摘要的属性。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceComplianceScriptRunSummary](../api/intune-devices-devicecompliancescriptrunsummary-get.md)|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|读取[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)对象的属性和关系。|
|[更新 deviceComplianceScriptRunSummary](../api/intune-devices-devicecompliancescriptrunsummary-update.md)|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|更新[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备符合性脚本运行摘要实体的键。 此属性是只读的。|
|noIssueDetectedDeviceCount|Int32|检测脚本找不到问题且设备正常运行的设备数量。 有效值-2147483648 到2147483647|
|issueDetectedDeviceCount|Int32|检测脚本发现问题的设备数。 有效值-2147483648 到2147483647|
|detectionScriptErrorDeviceCount|Int32|检测脚本执行时遇到错误且未完成的设备数量。 有效值-2147483648 到2147483647|
|detectionScriptPendingDeviceCount|Int32|尚未运行的设备符合性脚本的最新版本的设备数量。 有效值-2147483648 到2147483647|
|lastScriptRunDateTime|DateTimeOffset|在所有设备上的脚本的上次运行时间|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)"
}
```



