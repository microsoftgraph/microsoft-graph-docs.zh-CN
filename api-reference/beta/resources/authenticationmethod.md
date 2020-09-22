---
title: authenticationMethod 资源类型
description: 表示向用户注册的身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b9510a53ea80142bd9f155dce3e12824ad2d186e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034121"
---
# <a name="authenticationmethod-resource-type"></a>authenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示向用户注册的身份验证方法。 [身份验证方法](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods)是用户使用的一种方法，用于对系统进行身份验证或为其证明身份。 一些示例包括密码、电话 (可通过短信或语音呼叫) FIDO2 安全密钥等。 目前实施了密码和电话方法。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 authenticationMethods](../api/authentication-list-methods.md) | [authenticationMethod](authenticationmethod.md) 集合 | 读取用户的所有 **authenticationMethod** 对象的属性和关系。 |
| [获取 authenticationMethod](../api/authenticationmethod-get.md) | [authenticationMethod](authenticationmethod.md) | 读取 **authenticationMethod** 对象的属性和关系。 |

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


