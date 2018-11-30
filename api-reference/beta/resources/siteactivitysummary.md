---
title: siteActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 354b329f592964249590b2f551d66681f45de485
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045210"
---
# <a name="siteactivitysummary-resource-type"></a>siteActivitySummary 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| reportRefreshDate | 日期   |
| viewedOrEdited    | Int64  |
| 同步            | Int64  |
| sharedInternally  | Int64  |
| sharedExternally  | Int64  |
| reportDate        | 日期   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
