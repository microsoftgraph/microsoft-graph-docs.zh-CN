---
title: sharePointSiteUsagePages 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 1a1378bbe4ebaf1809aa641b22cde439f50d830b016b7cc393842f21cecbe029
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246082"
---
# <a name="sharepointsiteusagepages-resource-type"></a>sharePointSiteUsagePages 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| reportRefreshDate | 日期   |
| siteType          | 字符串 |
| pageViewCount     | Int64  |
| reportDate        | 日期   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsagePages"
} -->

```json
{
  "reportRefreshDate": "Date",
  "siteType": "String",
  "pageViewCount": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


