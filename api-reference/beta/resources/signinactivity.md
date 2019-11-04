---
title: signInActivity 资源类型
description: 提供特定用户的上次登录日期。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d93ff4f3b395d9b0820865c3293a419471ab6473
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939241"
---
# <a name="signinactivity-resource-type"></a>signInActivity 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供特定用户的上次登录日期。

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|lastSignInDateTime|DateTimeOffset|特定用户的上次登录日期。 您可以使用此字段来计算用户上次登录目录的时间。 此字段可用于生成报表，如非活动用户。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|lastSignInRequestId|字符串|此用户执行的最后一个登录的请求 ID。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInActivity",
  "baseType": null
}-->

```json
{
  "lastSignInDateTime": "String (timestamp)",
  "lastSignInRequestId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->