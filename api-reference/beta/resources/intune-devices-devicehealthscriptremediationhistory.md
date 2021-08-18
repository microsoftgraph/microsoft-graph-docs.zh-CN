---
title: deviceHealthScriptRemediationHistory 资源类型
description: 在给定日期和上次修改时间由设备运行状况脚本修正的设备数量。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 96840d696fdf85bced2b3f356f4322c5f912180dc10fddb2d983853e108f77ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54148041"
---
# <a name="devicehealthscriptremediationhistory-resource-type"></a>deviceHealthScriptRemediationHistory 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

在给定日期和上次修改时间由设备运行状况脚本修正的设备数量。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|为 healthscript 计算结果历史记录的日期。|
|historyData|[deviceHealthScriptRemediationHistoryData](../resources/intune-devices-devicehealthscriptremediationhistorydata.md) 集合|在给定日期由设备运行状况脚本修正的设备数量。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistory",
  "lastModifiedDateTime": "String (timestamp)",
  "historyData": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData",
      "date": "String (Date)",
      "remediatedDeviceCount": 1024,
      "noIssueDeviceCount": 1024
    }
  ]
}
```




