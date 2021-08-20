---
title: emailAppUsageVersionsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9b222982438be26c12e3e8b046f01c815a12f75775a170f2b9034c97d2897913
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54142230"
---
# <a name="emailappusageversionsusercounts-resource-type"></a>emailAppUsageVersionsUserCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| reportRefreshDate | 日期   |
| outlook2016       | Int64  |
| outlook2013       | Int64  |
| outlook2010       | Int64  |
| outlook2007       | Int64  |
| undetermined      | Int64  |
| reportPeriod      | 字符串 |
| outlookM365       | Int64  |
| outlook2019       | Int64  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "outlook2016": 1024, 
  "outlook2013": 1024, 
  "outlook2010": 1024, 
  "outlook2007": 1024, 
  "undetermined": 1024, 
  "reportPeriod": "String",
  "outlookM365": 1024,
  "outlook2019": 1024
}
```


