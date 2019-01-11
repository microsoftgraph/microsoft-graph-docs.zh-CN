---
title: office365GroupsActivityGroupCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: ed5386083b11fb6fe7f063a4890744532feeb081
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832618"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a>office365GroupsActivityGroupCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   | Description                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | 日期   | 内容最晚日期。          |
| total             | Int64  | 组的总数。              |
| 活动            | Int64  | 活动的组的数目。 组被视为活动发生以下任一： 组邮箱收到电子邮件;用户可以查看、 编辑、 共享，或同步中 SharePoint 文档库; 文件用户查看 SharePoint 页面; 例如：用户发布、 读取或喜欢 Yammer 组中的邮件。 |
| reportDate        | 日期   | 在其的组数处于活动状态日期。 |
| reportPeriod      | 字符串 | 报告涵盖天数。    |

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
