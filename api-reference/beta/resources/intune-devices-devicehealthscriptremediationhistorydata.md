---
title: deviceHealthScriptRemediationHistoryData 资源类型
description: 给定日期设备运行状况脚本修正的设备数量。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b9c04485659482d3f3ad28e3242bfb90b069a1d7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693736"
---
# <a name="devicehealthscriptremediationhistorydata-resource-type"></a>deviceHealthScriptRemediationHistoryData 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定日期设备运行状况脚本修正的设备数量。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|date|Date|设备运行状况脚本修正设备的日期。|
|remediatedDeviceCount|Int32|设备运行状况脚本修正的设备数。|
|noIssueDeviceCount|Int32|设备运行状况脚本发现没有问题的设备数量。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistoryData",
  "date": "String (Date)",
  "remediatedDeviceCount": 1024,
  "noIssueDeviceCount": 1024
}
```





