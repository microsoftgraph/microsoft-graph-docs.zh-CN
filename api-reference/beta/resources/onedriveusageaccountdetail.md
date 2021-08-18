---
title: oneDriveUsageAccountDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 210728ee77bb013a4894156aef79d35248e7d2f32eed129baf8905655f192f5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155972"
---
# <a name="onedriveusageaccountdetail-resource-type"></a>oneDriveUsageAccountDetail 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                | 类型    |
| :---------------------- | :------ |
| reportRefreshDate       | 日期    |
| siteUrl                 | 字符串  |
| ownerDisplayName        | 字符串  |
| ownerPrincipalName      | String  |
| isDeleted               | 布尔值 |
| lastActivityDate        | 日期    |
| fileCount               | Int64   |
| activeFileCount         | Int64   |
| storageUsedInBytes      | Int64   |
| storageAllocatedInBytes | Int64   |
| reportPeriod            | String  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date",
  "siteUrl": "String",
  "ownerDisplayName": "String",
  "ownerPrincipalName": "String",
  "isDeleted": true,
  "lastActivityDate": "Date",
  "fileCount": 1024,
  "activeFileCount": 1024,
  "storageUsedInBytes": 1024,
  "storageAllocatedInBytes": 1024,
  "reportPeriod": "String"
}
```


