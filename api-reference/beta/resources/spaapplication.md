---
title: spaApplication 资源类型
description: 指定单个页面应用程序的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: hamiltonha
ms.openlocfilehash: dd5e2c6419acd66cb482f2ccff2914b1bf0245dc
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031901"
---
# <a name="spaapplication-resource-type"></a>spaApplication 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定单个页面应用程序的设置。

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:---------|:-----|:------------|
| redirectUris | String collection | 指定向其发送用户令牌以进行登录的 Url，或用于发送 OAuth 2.0 授权代码和访问令牌的重定向 Uri。 |

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
