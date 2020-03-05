---
title: yammerGroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 9363bd711900cc6211e995c112581d3a91e08a04
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518985"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>yammerGroupsActivityDetail 资源类型

命名空间： microsoft. graph

## <a name="properties"></a>属性

| 属性           | 类型    |
| :----------------- | :------ |
| reportRefreshDate  | 日期    |
| groupDisplayName   | String  |
| isDeleted          | 布尔 |
| ownerPrincipalName | String  |
| lastActivityDate   | 日期    |
| groupType          | String  |
| office365Connected | 布尔 |
| memberCount        | Int64   |
| postedCount        | Int64   |
| readCount          | Int64   |
| likedCount         | Int64   |
| reportPeriod       | String  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "office365Connected": true, 
  "memberCount": 1024, 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "reportPeriod": "String"
}
```
