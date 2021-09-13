---
title: office365ActivationsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: c566383e339b4277b93fcd5177068f179626a570
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033292"
---
# <a name="office365activationsusercounts-resource-type"></a>office365ActivationsUserCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                 | 类型   | 描述                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | 日期   | 内容的最新日期。          |
| productType              | String | 产品类型，例如"Microsoft 365 ProPlus"或"Project Client"。 |
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


