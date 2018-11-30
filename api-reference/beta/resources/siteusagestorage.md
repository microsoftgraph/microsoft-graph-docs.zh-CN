---
title: siteUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 1fdfa6cb2690d6dbacf5e534792061b6e64025d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042718"
---
# <a name="siteusagestorage-resource-type"></a>siteUsageStorage 资源类型

## <a name="properties"></a>属性

| 属性           | 类型   |
| :----------------- | :----- |
| reportRefreshDate  | 日期   |
| 键入一个文件夹           | 字符串 |
| storageUsedInBytes | Int64  |
| reportDate         | 日期   |
| reportPeriod       | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
