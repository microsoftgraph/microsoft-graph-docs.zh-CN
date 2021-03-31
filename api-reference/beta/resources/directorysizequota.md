---
title: directorySizeQuota 资源类型
description: 表示公司使用的目录配额和总目录配额。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: 54e2280fdb416e5ccfd0853ee77a2ef3f90ddf37
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469372"
---
# <a name="directorysizequota-resource-type"></a>directorySizeQuota 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示公司使用的目录配额和总目录配额。

## <a name="properties"></a>属性
| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|使用的内容|Int32| 已使用的目录配额量。 |
|total|Int32| 目录配额的总量。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySizeQuota"
}-->

```json
{
  "used": 123,
  "total": 1234
}
```
