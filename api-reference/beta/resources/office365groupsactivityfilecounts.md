---
title: office365GroupsActivityFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: eb2d967108d4f75064b91670ae43fb7a2dd7ce7a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042666"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>office365GroupsActivityFileCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   | 说明                              |
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
