---
title: dailySchedule 资源类型
description: 定期设备管理脚本的每日运行计划。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd2b226255f433b4f82d042b6389830143515033
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788070"
---
# <a name="dailyschedule-resource-type"></a>dailySchedule 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

定期设备管理脚本的每日运行计划。


继承自[runSchedule](../resources/intune-devices-runschedule.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|interval|Int32|以天为单位的时间间隔|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dailySchedule",
  "interval": 1024
}
```





