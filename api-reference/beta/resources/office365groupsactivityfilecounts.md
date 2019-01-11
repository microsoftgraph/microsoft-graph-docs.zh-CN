---
title: office365GroupsActivityFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 856bb4c74c8af35775b6fe71cb75d89935440bdb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819183"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>office365GroupsActivityFileCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   | Description                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | 日期   | 内容最晚日期。          |
| total             | Int64  | 组的 SharePoint 文档库中的文件总数。 |
| 活动            | Int64  | 查看过的文件数编辑、 共享，或组的 SharePoint 文档库同步。 |
| reportDate        | 日期   | 在其的文件数处于活动状态的组的 SharePoint 网站中的日期。 |
| reportPeriod      | 字符串 | 报告涵盖天数。    |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {

  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
