---
title: optionalClaim 资源类型
description: 在此处提供说明
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 91d110f47b9d3a95b32173bb1b8b8880799d6d11
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104101"
---
# <a name="optionalclaim-resource-type"></a>optionalClaim 资源类型

命名空间：microsoft.graph

包含与应用程序关联的可选 [声明](application.md) <!-- or a service principal -->. optionalClaims 资源的 、 和 属性 `idToken` `accessToken` 是 `saml2Token` **optionalClaim 的集合**。 [](optionalclaims.md) 如果受特定声明支持，您还可以使用 属性修改 optionalClaim `additionalProperties` 的行为。

有关详细信息，请参阅[向 Azure AD 应用提供可选声明](/azure/active-directory/develop/active-directory-optional-claims)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|additionalProperties|String collection| 声明的其他属性。 如果此集合中存在属性，则它会修改 name 属性中指定的可选声明的行为。 |
|essential|布尔值| 如果值为 true，则客户端指定的声明是确保最终用户请求的特定任务的流畅授权体验所必需的。 默认值为 false。|
|name|String| 可选声明的名称。 |
|source|String| 源 (声明) 目录对象。 存在来自扩展属性的预定义声明和用户定义的声明。 如果源值为 null，则声明为预定义的可选声明。 如果源值为 user，name 属性中的值为 user 对象的扩展属性。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.optionalClaim",
  "baseType": null
}-->

```json
{
  "additionalProperties": ["String"],
  "essential": true,
  "name": "String",
  "source": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "optionalClaim resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
