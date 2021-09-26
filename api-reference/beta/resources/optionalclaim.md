---
title: optionalClaim 资源类型
description: 包含与应用程序关联的可选声明。
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: b4816822928cab9f84dbbdc60e13a6ceab6ef26b
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767137"
---
# <a name="optionalclaim-resource-type"></a>optionalClaim 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含与应用程序关联的可选 [声明](application.md) <!-- or a service principal -->. [optionalClaims](optionalclaims.md)资源的 **idToken、accessToken** 和 **saml2Token** 属性是 **optionalClaim 的集合**。  如果受特定声明支持，您还可以使用 属性修改 optionalClaim `additionalProperties` 的行为。 

有关详细信息，请参阅向 [Azure AD 应用提供可选声明](/azure/active-directory/develop/active-directory-optional-claims)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|additionalProperties|String collection| 声明的其他属性。 如果此集合中存在属性，则它会修改 name 属性中指定的可选声明的行为。 |
|essential|Boolean| 如果值为 true，则客户端指定的声明是确保最终用户请求的特定任务的流畅授权体验所必需的。 默认值为 false。|
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
