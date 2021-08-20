---
title: deviceHealthScriptRunOnceSchedule 资源类型
description: 设备运行状况脚本运行一次计划。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 324b8c0ced6c2e10da4dfd0a60c6d4c4aa26d2140176cd85f35527769daadf39
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206366"
---
# <a name="devicehealthscriptrunonceschedule-resource-type"></a>deviceHealthScriptRunOnceSchedule 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备运行状况脚本运行一次计划。


继承自 [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|interval|Int32|每小时计划每 x 小时、每 x 天（每日计划每 x 天、每周计划每 x 周、每月计划每 x 个月）的 x 值。 有效值 1 到 23 继承自 [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|
|useUtc|布尔值|指示时间是 Utc 还是客户端本地时间。 继承自 [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)|
|time|TimeOfDay|计划运行脚本的时间。 此集合最多可包含 20 个元素。 继承自 [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)|
|date|Date|脚本计划运行的日期。 此集合最多可包含 20 个元素。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunOnceSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunOnceSchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)",
  "date": "String (Date)"
}
```




