---
title: yammerActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d24e21c9525d49b7af5f8c4efaddd606c20c162b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923031"
---
# <a name="yammeractivityuserdetail-resource-type"></a>yammerActivityUserDetail 资源类型

## <a name="properties"></a>属性

| 属性          | 类型              |
| :---------------- | :---------------- |
| reportRefreshDate | 日期              |
| userPrincipalName | 字符串            |
| displayName       | 字符串            |
| userState         | 字符串            |
| stateChangeDate   | 日期              |
| lastActivityDate  | 日期              |
| postedCount       | Int64             |
| readCount         | Int64             |
| likedCount        | Int64             |
| assignedProducts  | String 集合 |
| reportPeriod      | String            |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
