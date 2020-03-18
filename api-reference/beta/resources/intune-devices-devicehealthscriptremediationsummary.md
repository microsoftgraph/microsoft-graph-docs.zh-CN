---
title: deviceHealthScriptRemediationSummary 资源类型
description: 已部署的设备运行状况脚本数以及脚本修正的设备数。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b59f2d057f258e60a8182194c1ac930e95012b93
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784942"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a>deviceHealthScriptRemediationSummary 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

已部署的设备运行状况脚本数以及脚本修正的设备数。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|scriptCount|Int32|已部署的设备运行状况脚本的数量。|
|remediatedDeviceCount|Int32|设备运行状况脚本修正的设备数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationSummary",
  "scriptCount": 1024,
  "remediatedDeviceCount": 1024
}
```



