---
title: office365GroupsActivityStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505548"
---
# <a name="office365groupsactivitystorage-resource-type"></a>office365GroupsActivityStorage 资源类型

## <a name="properties"></a>属性

| 属性                  | 类型   | 说明                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | Date   | 内容的最新日期。          |
| mailboxStorageUsedInBytes | Int64  | 组邮箱中使用的存储。       |
| siteStorageUsedInBytes    | Int64  | SharePoint 文档库中使用的存储区。 |
| reportDate                | Date   | Exchange 和 SharePoint 使用的存储的快照日期。 |
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
