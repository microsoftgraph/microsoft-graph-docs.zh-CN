---
title: deviceComplianceScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84bd44e53266976564f2eb4bb5ea6277cba0208c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033558"
---
# <a name="devicecompliancescriptrunsummary-resource-type"></a>deviceComplianceScriptRunSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含设备管理脚本的运行摘要的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceComplianceScriptRunSummary](../api/intune-devices-devicecompliancescriptrunsummary-get.md)|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|读取 [deviceComplianceScriptRunSummary 对象的属性和](../resources/intune-devices-devicecompliancescriptrunsummary.md) 关系。|
|[更新 deviceComplianceScriptRunSummary](../api/intune-devices-devicecompliancescriptrunsummary-update.md)|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|更新 [deviceComplianceScriptRunSummary 对象](../resources/intune-devices-devicecompliancescriptrunsummary.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备合规性脚本运行摘要实体的密钥。 此属性是只读的。|
|noIssueDetectedDeviceCount|Int32|检测脚本未发现问题且设备正常运行的设备数量。 有效值 -2147483648 2147483647|
|issueDetectedDeviceCount|Int32|检测脚本发现问题的设备数量。 有效值 -2147483648 2147483647|
|detectionScriptErrorDeviceCount|Int32|检测脚本执行遇到错误且未完成的设备数量。 有效值 -2147483648 2147483647|
|detectionScriptPendingDeviceCount|Int32|尚未运行最新版本的设备合规性脚本的设备数量。 有效值 -2147483648 2147483647|
|lastScriptRunDateTime|DateTimeOffset|脚本跨所有设备的上次运行时间|

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



