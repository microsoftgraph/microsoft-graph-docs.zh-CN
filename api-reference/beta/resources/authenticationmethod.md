---
title: authenticationMethod 资源类型
description: 表示向用户注册的身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d1c43525352411a4b27952be4e6592401d28c54b
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874324"
---
# <a name="authenticationmethod-resource-type"></a>authenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示向用户注册的身份验证方法。 [身份验证方法是](/azure/active-directory/authentication/concept-authentication-methods)用户用来向系统进行身份验证或以其他方式证明其身份的方法。 一些示例包括密码、 (短信或语音呼叫) 、FIDO2 安全密钥等。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [列出 authenticationMethods](../api/authentication-list-methods.md) | [authenticationMethod](authenticationmethod.md) 集合 | 读取用户的所有 **authenticationMethod** 对象的属性和关系。 |
| [获取 authenticationMethod](../api/authenticationmethod-get.md) | [authenticationMethod](authenticationmethod.md) | 读取 **authenticationMethod 对象的属性和** 关系。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 向此用户注册的身份验证方法的此实例的标识符。 只读。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationMethod",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->