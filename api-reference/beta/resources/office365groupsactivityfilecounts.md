---
title: office365GroupsActivityFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 89ac23b89730ec98515d6d0d3c06867e57b19ed1
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575574"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>office365GroupsActivityFileCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   | 说明                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Date   | 内容最晚日期。          |
| total             | Int64  | 组的 SharePoint 文档库中的文件总数。 |
| 活动            | Int64  | 查看过的文件数编辑、 共享，或组的 SharePoint 文档库同步。 |
| reportDate        | Date   | 在其的文件数处于活动状态的组的 SharePoint 网站中的日期。 |
| reportPeriod      | String | 报告涵盖天数。    |

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
