---
title: deviceHealthScriptRemediationHistoryData 资源类型
description: 在给定日期由设备运行状况脚本修正的设备数量。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c6c456b3edc591c0394446bbb23b6975781da4d4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793808"
---
# <a name="devicehealthscriptremediationhistorydata-resource-type"></a>deviceHealthScriptRemediationHistoryData 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

在给定日期由设备运行状况脚本修正的设备数量。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|date|Date|设备运行状况脚本修正设备的日期。|
|remediatedDeviceCount|Int32|由设备运行状况脚本修正的设备数量。|
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



