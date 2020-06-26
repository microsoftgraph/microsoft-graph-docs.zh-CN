---
title: office365ActivationsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: b8746d58b03b15a3118e8fc51a42e61e3c22cb78
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896803"
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
