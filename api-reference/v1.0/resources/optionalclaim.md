---
title: optionalClaim 资源类型
description: 在此处提供说明
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 0a7b6072b53fe26384f82f706b694c4b04c33113
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128349"
---
# <a name="optionalclaim-resource-type"></a>optionalClaim 资源类型

命名空间：microsoft.graph

包含与应用程序关联的可选 [声明](application.md) <!-- or a service principal -->. optionalClaims 资源的 ， `idToken` `accessToken` `saml2Token` 和属性是 **optionalClaim 的集合**。 [](optionalclaims.md) 如果特定声明支持，您还可以使用该属性修改 optionalClaim `additionalProperties` 的行为。

有关详细信息，请参阅[向 Azure AD 应用提供可选声明](/azure/active-directory/develop/active-directory-optional-claims)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|additionalProperties|String collection| 声明的其他属性。 如果属性存在于该集合中，则它会修改在 name 属性中指定的可选声明的行为。 |
|essential|布尔| 如果值为 true，则客户端指定的声明是确保最终用户请求的特定任务的流畅授权体验所必需的。 默认值为 false。|
|name|String| 可选声明的名称。 |
|source|String| 源 (声明) 目录对象。 扩展属性中具有预定义声明和用户定义的声明。 如果源值为空，则声明是预定义的可选声明。 如果源值是用户，则 name 属性中的值是用户对象的扩展属性。 |

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
