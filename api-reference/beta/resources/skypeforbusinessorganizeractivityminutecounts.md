---
title: skypeForBusinessOrganizerActivityMinuteCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 6b3b38c61ebb7b294de9ea5fc2641a7527bf04f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823203"
---
# <a name="skypeforbusinessorganizeractivityminutecounts-resource-type"></a>skypeForBusinessOrganizerActivityMinuteCounts 资源类型

## <a name="properties"></a>属性

| 属性           | 类型   |
| :----------------- | :----- |
| audioVideo         | Int64  |
| dialInOut3rdParty  | Int64  |
| dialInOutMicrosoft | Int64  |
| reportRefreshDate  | 日期   |
| reportDate         | 日期   |
| reportPeriod       | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```json
{
  "audioVideo": 1024, 
  "dialInMicrosoft": 1024, 
  "dialOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
