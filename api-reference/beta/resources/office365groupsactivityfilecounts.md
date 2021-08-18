---
title: office365GroupsActivityFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: f05cf16e1b2e0273aaa62241bbeac3b0d872bf87605e2c852ac2ab28e25f9526
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54160861"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>office365GroupsActivityFileCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型   | 说明                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | 日期   | 内容的最新日期。          |
| total             | Int64  | 组的文档库中的文件SharePoint总数。 |
| active            | Int64  | 在组的文档库中查看、编辑、共享或同步SharePoint的数量。 |
| reportDate        | 日期   | 在组的网站中激活多个文件SharePoint的日期。 |
| reportPeriod      | String | 报告涵盖的天数。    |

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


