---
title: skypeForBusinessOrganizerActivityMinuteCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: ba19256ad7359699e881aa47fb0e1eaaad2f80250ad00fd13a775614ff10e923
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54241266"
---
# <a name="skypeforbusinessorganizeractivityminutecounts-resource-type"></a>skypeForBusinessOrganizerActivityMinuteCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性           | 类型   |
| :----------------- | :----- |
| audioVideo         | Int64  |
| dialInMicrosoft    | Int64  |
| dialOutMicrosoft   | Int64  |
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


