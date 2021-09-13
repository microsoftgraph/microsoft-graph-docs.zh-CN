---
title: sharePointSiteUsageFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: ebe4eb3b7f357d45de6afd2efc662a8ba80c6d20
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038788"
---
# <a name="sharepointsiteusagefilecounts-resource-type"></a>sharePointSiteUsageFileCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| reportRefreshDate | 日期   |
| siteType          | String |
| total             | Int64  |
| active            | Int64  |
| reportDate        | 日期   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageFileCounts"
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


