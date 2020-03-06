---
title: yammerGroupsActivityGroupCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 426b3e2a6be72c0cc87d4c284b56fd83b1c12141
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518978"
---
# <a name="yammergroupsactivitygroupcounts-resource-type"></a>yammerGroupsActivityGroupCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型   | 说明 |
| :---------------- | :----- | :---------- |
| reportRefreshDate | 日期   |             |
| total             | Int64  |             |
| 工作            | Int64  |             |
| reportDate        | 日期   |             |
| reportPeriod      | 字符串 |             |

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
