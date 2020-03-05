---
title: emailActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: dd30bb496cb6591b3bde11d1c0c38b4099175891
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499587"
---
# <a name="emailactivitysummary-resource-type"></a>emailActivitySummary 资源类型

命名空间： microsoft. graph

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| reportRefreshDate | 日期   |
| 发送              | Int64  |
| 享受           | Int64  |
| 自述              | Int64  |
| reportDate        | 日期   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
