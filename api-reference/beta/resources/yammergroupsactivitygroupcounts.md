---
title: yammerGroupsActivityGroupCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 64947a1d151cab3dca14f4f232671242e1a985cc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342728"
---
# <a name="yammergroupsactivitygroupcounts-resource-type"></a>yammerGroupsActivityGroupCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   | 说明 |
| :---------------- | :----- | :---------- |
| reportRefreshDate | Date   |             |
| total             | Int64  |             |
| 工作            | Int64  |             |
| reportDate        | Date   |             |
| reportPeriod      | String |             |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityGroupCounts"
} -->

```json
{
  "reportRefreshDate": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "String", 
  "reportPeriod": "String"
}
```
