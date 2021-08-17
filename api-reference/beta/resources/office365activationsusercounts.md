---
title: office365ActivationsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: de01adee754940bd43be258b4454b7c68c0e4f8254581486d59a34f9a1f06478
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139142"
---
# <a name="office365activationsusercounts-resource-type"></a>office365ActivationsUserCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                 | 类型   | 说明                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | 日期   | 内容的最新日期。          |
| productType              | 字符串 | 产品类型，如"Microsoft 365 ProPlus"或"Project Client"。 |
| 已分配                 | Int64  | 为产品许可证分配的用户数。 |
| activated                | Int64  | 已激活产品的用户数。 |
| sharedComputerActivation | Int64  | 在共享计算机上使用产品的用户数。 |

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


