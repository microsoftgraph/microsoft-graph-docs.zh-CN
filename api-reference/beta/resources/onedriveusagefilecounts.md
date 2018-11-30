---
title: oneDriveUsageFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 98e387b97687a4aab55e8d94e72fdbfa585a0e84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042382"
---
# <a name="onedriveusagefilecounts-resource-type"></a>oneDriveUsageFileCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| reportRefreshDate | 日期   |
| 键入一个文件夹          | 字符串 |
| total             | Int64  |
| 活动            | Int64  |
| reportDate        | 日期   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
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
