---
title: deviceHealthScriptHourlySchedule 资源类型
description: 每小时计划的设备运行状况脚本的类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6128f3d16a3d64858871903131e4c799de03415d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023470"
---
# <a name="devicehealthscripthourlyschedule-resource-type"></a>deviceHealthScriptHourlySchedule 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

每小时计划的设备运行状况脚本的类型。


继承自 [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|interval|Int32|每小时计划的每 x 小时、每天计划每 x 天、每周计划每 x 周、每月计划每 x 个月的 x 值。 有效值 1 到 23 继承自 [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptHourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptHourlySchedule",
  "interval": 1024
}
```



