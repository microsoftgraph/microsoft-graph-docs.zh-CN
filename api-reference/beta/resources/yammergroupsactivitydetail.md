---
title: yammerGroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 7c3b10b7b96c40ae7b7404eee2c9af99ea4bc2d602c93f9f6c68ef2ed7ad8cbe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54176083"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>yammerGroupsActivityDetail 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性           | 类型    |
| :----------------- | :------ |
| reportRefreshDate  | 日期    |
| groupDisplayName   | 字符串  |
| isDeleted          | 布尔值 |
| ownerPrincipalName | 字符串  |
| lastActivityDate   | 日期    |
| groupType          | 字符串  |
| office365Connected | 布尔值 |
| memberCount        | Int64   |
| postedCount        | Int64   |
| readCount          | Int64   |
| likedCount         | Int64   |
| networkDisplayName | 字符串  |
| reportPeriod       | 字符串  |

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
  "networkDisplayName": "String",
  "reportPeriod": "String"
}
```


