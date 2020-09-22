---
title: office365ActivationsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 21e18b35dc4e4ff639087617d679ae1583516026
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021222"
---
# <a name="office365activationsusercounts-resource-type"></a>office365ActivationsUserCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                 | 类型   | 说明                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | 日期   | 内容的最新日期。          |
| productType              | String | 产品类型，如 "Microsoft 365 专业增强版" 或 "Project Client"。 |
| 赋予                 | Int64  | 已为产品许可证分配了用户数量。 |
| 已                | Int64  | 激活产品的用户数。 |
| sharedComputerActivation | Int64  | 在共享计算机上使用该产品的用户数。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "assigned": 1024, 
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```


