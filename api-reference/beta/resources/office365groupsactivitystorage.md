---
title: office365GroupsActivityStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 7ac9ca260e4723f7c4aeca8e15f837d4cd57b7c4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982178"
---
# <a name="office365groupsactivitystorage-resource-type"></a>office365GroupsActivityStorage 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                  | 类型   | 说明                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | 日期   | 内容的最新日期。          |
| mailboxStorageUsedInBytes | Int64  | 组邮箱中使用的存储。       |
| siteStorageUsedInBytes    | Int64  | SharePoint 文档库中使用的存储。 |
| reportDate                | 日期   | Exchange 和 SharePoint 使用的存储的快照日期。 |
| reportPeriod              | String | 报告涵盖的天数。    |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailboxStorageUsedInBytes": 1024, 
  "siteStorageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


