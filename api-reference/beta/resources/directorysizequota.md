---
title: directorySizeQuota 资源类型
description: 表示公司使用的目录配额和总目录配额。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: ac8b26fababe53458b8dd3a92624d9ce0a11514a
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60483013"
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
  "used": "Int32",
  "total": "Int32"
}
```
