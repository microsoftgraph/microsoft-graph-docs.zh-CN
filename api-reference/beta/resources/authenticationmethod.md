---
title: authenticationMethod 资源类型
description: 表示注册到用户的身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9ab808934491793b796be1c66fc87051ed6e9b29
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335623"
---
# <a name="authenticationmethod-resource-type"></a>authenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示注册到用户的身份验证方法。 [身份验证方法是](/azure/active-directory/authentication/concept-authentication-methods)用户用来向系统进行身份验证或以其他方式证明其身份的方法。 一些示例包括密码、 (电话短信或语音呼叫) 、FIDO2 安全密钥等。

> [!IMPORTANT]
> 列出用户的身份验证方法仅返回此 API 版本支持的方法。 有关 [当前支持的方法的列表，请参阅 Azure AD 身份验证](authenticationmethods-overview.md) 方法 API 概述。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 authenticationMethods](../api/authentication-list-methods.md) | [authenticationMethod](authenticationmethod.md) 集合 | 读取用户的所有 **authenticationMethod** 对象的属性和关系。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 注册到此用户的身份验证方法的此实例的标识符。 只读。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationMethod",
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