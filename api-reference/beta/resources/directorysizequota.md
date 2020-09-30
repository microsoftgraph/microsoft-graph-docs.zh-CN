---
title: directorySizeQuota 资源类型
description: 表示公司的已用和总目录配额。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 8f5f172cb8f090b71b7e0fd3c89151668c167afd
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315597"
---
# <a name="directorysizequota-resource-type"></a>directorySizeQuota 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示公司的已用和总目录配额。

## <a name="properties"></a>属性
| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|使用的内容|Int32| 已用的目录配额量。 |
|total|Int32| 目录配额总量。|

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
