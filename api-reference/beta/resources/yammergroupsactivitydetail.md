---
title: yammerGroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 1cb26b450d5007caf42521a2265c25a57c8d7793
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128471"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>yammerGroupsActivityDetail 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性           | 类型    |
| :----------------- | :------ |
| reportRefreshDate  | 日期    |
| groupDisplayName   | String  |
| isDeleted          | Boolean |
| ownerPrincipalName | String  |
| lastActivityDate   | 日期    |
| groupType          | String  |
| office365Connected | Boolean |
| memberCount        | Int64   |
| postedCount        | Int64   |
| readCount          | Int64   |
| likedCount         | Int64   |
| networkDisplayName | String  |
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
  "networkDisplayName": "String",
  "reportPeriod": "String"
}
```


