---
title: spaApplication 资源类型
description: 指定单页应用程序的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: hamiltonha
ms.openlocfilehash: a05d2eb997212b3baf88b84e21468475a45a691c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128825"
---
# <a name="spaapplication-resource-type"></a>spaApplication 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定单页应用程序的设置。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| redirectUris | 字符串集合 | 指定用于登录的用户令牌的发送 URL，或发送 OAuth 2.0 授权代码和访问令牌的重定向 URI。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.spaApplication"
}-->

```json
{
  "redirectUris": ["String"]
}
```
