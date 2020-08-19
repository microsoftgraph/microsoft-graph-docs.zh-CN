---
title: skypeForBusinessOrganizerActivityMinuteCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 923d8a54ed2d43764ed05e47fe2e26516f1536ac
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811061"
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
