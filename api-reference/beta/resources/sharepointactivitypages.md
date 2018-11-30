---
title: sharePointActivityPages 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 9111457d5cb9e710f0b07a43ea06c137af0db0f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041510"
---
# <a name="sharepointactivitypages-resource-type"></a>sharePointActivityPages 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| reportRefreshDate | 日期   |
| visitedPageCount  | Int64  |
| reportDate        | 日期   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityPages"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "visitedPageCount": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
