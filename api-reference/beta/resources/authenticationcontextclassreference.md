---
title: authenticationContextClassReference 资源类型
description: 表示一Azure Active Directory身份验证上下文类引用。
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1397545d7b102d05b8c71957cea88f9c131f0e09
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547412"
---
# <a name="authenticationcontextclassreference-resource-type"></a>authenticationContextClassReference 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一Azure Active Directory身份验证上下文类引用。 身份验证上下文类引用是定义条件访问身份验证要求的自定义值。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 authenticationContextClassReference](../api/conditionalaccessroot-list-authenticationcontextclassreferences.md) | [authenticationContextClassReference](authenticationContextClassReference.md) 集合 | 获取组织的所有 authenticationContextClassReference 对象。 |
| [创建 authenticationContextClassReference](../api/conditionalaccessroot-post-authenticationcontextclassreferences.md) | [authenticationContextClassReference](authenticationContextClassReference.md) | 创建新的 authenticationContextClassReference 对象。 |
| [获取 authenticationContextClassReference](../api/authenticationcontextclassreference-get.md) | [authenticationContextClassReference](authenticationContextClassReference.md) | 读取 authenticationContextClassReference 对象的属性和关系。 |
| [更新 authenticationContextClassReference](../api/authenticationcontextclassreference-update.md) | [authenticationContextClassReference](authenticationContextClassReference.md) | 更新 authenticationContextClassReference 对象。 |


## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 用于引用身份验证上下文类的标识符。 id 用于触发引用的身份验证要求的逐步身份验证，它是将在 acrs 声明中发出的值。 声明中的此值用于验证是否满足所需的身份验证上下文。 允许的 id 值为"c1"到"c25"。 |
|displayName|String| the 显示名称 is the friendly name of the authenticationContextClassReference. 此值应该用于在构建面向用户的管理员体验时标识身份验证上下文类引用。 例如，选择 UX。 |
|说明|String| authenticationContextClassReference 强制执行的策略的简短说明。 此值应该用于提供辅助文本，以在构建面向用户的管理员体验时描述身份验证上下文类引用。 例如，选择 UX。|
|isAvailable|boolean| 指示 authenticationContextClassReference 是否已由安全管理员发布，并可供应用使用。 如果设置为 ，则不应在管理员 UX 体验中显示该值，因为该值 `false` 当前不能用于选择。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "description",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.authenticationContextClassReference",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id"
}-->

```json
    {
      "id": "String",
      "displayName": "String",
      "description": "String",
      "isAvailable": "boolean",
    }

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationContextClassReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
