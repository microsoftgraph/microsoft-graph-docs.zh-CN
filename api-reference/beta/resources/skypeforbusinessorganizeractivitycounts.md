---
title: skypeForBusinessOrganizerActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 1289e1001a8d6b3cdb2cba69aa85b1b1c31cc023c71b0d0b802adc39c3c2ebd5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54241287"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a>skypeForBusinessOrganizerActivityCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性           | 类型   |
| :----------------- | :----- |
| 即时消息                 | Int64  |
| audioVideo         | Int64  |
| appSharing         | Int64  |
| web                | Int64  |
| dialInOut3rdParty  | Int64  |
| dialInOutMicrosoft | Int64  |
| reportRefreshDate  | 日期   |
| reportDate         | 日期   |
| reportPeriod       | 字符串 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```json
{
  "im": 1024,
  "audioVideo": 1024,
  "appSharing": 1024,
  "web": 1024,
  "dialInOut3rdParty": 1024,
  "dialInOutMicrosoft": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


