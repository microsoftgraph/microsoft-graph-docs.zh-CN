---
title: office365GroupsActivityStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 0b14e6981a193ad1698303d2762d0321de430b73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092389"
---
# <a name="office365groupsactivitystorage-resource-type"></a>office365GroupsActivityStorage 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                  | 类型   | 说明                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | 日期   | 内容的最新日期。          |
| mailboxStorageUsedInBytes | Int64  | 组邮箱中使用的存储。       |
| siteStorageUsedInBytes    | Int64  | SharePoint 文档库中使用的存储区。 |
| reportDate                | 日期   | Exchange 和 SharePoint 使用的存储的快照日期。 |
| reportPeriod              | 字符串 | 报告覆盖的天数。    |

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


