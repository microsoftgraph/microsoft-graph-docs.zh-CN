---
title: office365GroupsActivityStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 9824d3d172a8578f8a25a049c2d0d3b407bbc47e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862249"
---
# <a name="office365groupsactivitystorage-resource-type"></a>office365GroupsActivityStorage 资源类型

## <a name="properties"></a>属性

| 属性                  | 类型   | Description                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | 日期   | 内容最晚日期。          |
| mailboxStorageUsedInBytes | Int64  | 使用组邮箱中的存储。       |
| siteStorageUsedInBytes    | Int64  | 在 SharePoint 文档库中使用的存储。 |
| reportDate                | 日期   | Exchange 和 SharePoint 的快照日期用于存储。 |
| reportPeriod              | 字符串 | 报告涵盖天数。    |

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
