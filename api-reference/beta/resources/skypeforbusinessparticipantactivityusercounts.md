---
title: skypeForBusinessParticipantActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: d65d7fd9c2c3389e47a8b1f94538be158efd2642
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045214"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a>skypeForBusinessParticipantActivityUserCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| im                | Int64  |
| audioVideo        | Int64  |
| 的        | Int64  |
| web               | Int64  |
| dialInOut3rdParty | Int64  |
| reportRefreshDate | 日期   |
| reportDate        | 日期   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 196, 
  "appSharing": 196, 
  "web": 196, 
  "dialInOut3rdParty": 196, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
