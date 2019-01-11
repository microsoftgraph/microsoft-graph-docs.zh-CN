---
title: office365ActivationsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: f57393a538631664be8845fdaeda9f35d07c986f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849306"
---
# <a name="office365activationsusercounts-resource-type"></a>office365ActivationsUserCounts 资源类型

## <a name="properties"></a>属性

| 属性                 | 类型   | Description                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | 日期   | 内容最晚日期。          |
| productType              | 字符串 | 产品类型，如"Office 365 ProPlus"、"Project 客户端"或"Visio Pro for Office 365"。 |
| 分配                 | Int64  | 产品许可证已分配的用户数。 |
| 激活                | Int64  | 已激活产品的用户数。 |
| sharedComputerActivation | Int64  | 共享计算机使用该产品的用户数。 |

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
