---
title: office365GroupsActivityFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: c887ecb526d9c4215c1d8586bcbcb799c9e2c476
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092403"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>office365GroupsActivityFileCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型   | 说明                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | 日期   | 内容的最新日期。          |
| total             | Int64  | 组的 SharePoint 文档库中的总文件数。 |
| 工作            | Int64  | 在组的 SharePoint 文档库中查看、编辑、共享或同步的文件数。 |
| reportDate        | 日期   | 组的 SharePoint 网站中处于活动状态的多个文件的日期。 |
| reportPeriod      | 字符串 | 报告覆盖的天数。    |

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


