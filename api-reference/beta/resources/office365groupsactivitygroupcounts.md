---
title: office365GroupsActivityGroupCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: b7f38f2279e7cd575972d13ea411d972349131a4fe3a9943c4e5efa03365ffa2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178708"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a>office365GroupsActivityGroupCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型   | 说明                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | 日期   | 内容的最新日期。          |
| total             | Int64  | 组总数。              |
| active            | Int64  | 活动组的数量。 如果发生以下任一情况，则认为组处于活动状态：组邮箱收到电子邮件;用户在文档库中查看、编辑、共享或同步SharePoint文件;用户查看SharePoint页面;用户发布、阅读或点过Yammer组。 |
| reportDate        | 日期   | 多个组处于活动状态的日期。 |
| reportPeriod      | String | 报告涵盖的天数。    |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
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


