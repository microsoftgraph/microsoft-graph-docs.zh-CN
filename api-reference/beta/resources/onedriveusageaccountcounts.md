---
title: oneDriveUsageAccountCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 770968141305275f33609db3deca8bb77f5d51cf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039312"
---
# <a name="onedriveusageaccountcounts-resource-type"></a>oneDriveUsageAccountCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| reportRefreshDate | 日期   |
| siteType          | String |
| total             | Int64  |
| 工作            | Int64  |
| reportDate        | 日期   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```json
{
  "reportRefreshDate": "Date",
  "siteType": "String",
  "total": 1024,
  "active": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


