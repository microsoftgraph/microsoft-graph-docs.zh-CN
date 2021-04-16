---
title: spaApplication 资源类型
description: 指定单页应用程序的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 25f907aa8c7e5b47960bb3a482b9745c488d16a9
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836982"
---
# <a name="spaapplication-resource-type"></a>spaApplication 资源类型

命名空间：microsoft.graph

指定单页应用程序的设置。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| redirectUris | String 集合 | 指定用于登录的用户令牌的 URL，或发送 OAuth 2.0 授权代码和访问令牌的重定向 URI。 |

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
