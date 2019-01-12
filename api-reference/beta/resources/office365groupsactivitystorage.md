---
title: office365GroupsActivityStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 180e60a52b397f969aa10cee5bc27bba934ad1e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944451"
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
