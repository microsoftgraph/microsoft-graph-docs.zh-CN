---
title: mailboxUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 8cc26c5d3cc30529857ed3273f8ee66c7373327a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043169"
---
# <a name="mailboxusagestorage-resource-type"></a>mailboxUsageStorage 资源类型

## <a name="properties"></a>属性

| 属性           | 类型   |
| :----------------- | :----- |
| reportRefreshDate  | 日期   |
| storageUsedInBytes | Int64  |
| reportDate         | 日期   |
| reportPeriod       | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
