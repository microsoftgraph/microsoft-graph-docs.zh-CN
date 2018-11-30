---
title: skypeForBusinessActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: eee736958540f2a3fb42cf3c76a37da4ebe78afd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049496"
---
# <a name="skypeforbusinessactivityusercounts-resource-type"></a>skypeForBusinessActivityUserCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| peerToPeer        | Int64  |
| 组织         | Int64  |
| 则参与了会议      | Int64  |
| reportRefreshDate | 日期   |
| reportDate        | 日期   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
} -->

```json
{
  "peerToPeer": 1024, 
  "organized": 1024, 
  "participated": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
