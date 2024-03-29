---
title: optionalClaims 类型
description: 声明应用程序请求的可选声明。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 11d504a24e438e4c11327838f302b1737818e12e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104094"
---
# <a name="optionalclaims-resource-type"></a>optionalClaims 资源类型

命名空间：microsoft.graph 声明应用程序请求的可选声明。 应用程序可以将可选声明配置为在三种类型的令牌中返回 (ID 令牌、访问令牌、SAML 2 令牌) 它可以从安全令牌服务接收。 应用程序可以配置一组不同的可选声明，以在每个令牌类型中返回。 应用程序的 optionalClaims 属性 [是](application.md)**一个可选的Claims** 对象。

应用程序开发人员可以在其 Azure AD 应用中配置可选声明，以指定 Microsoft 安全令牌服务发送到他们应用程序的令牌中所需的声明。 有关详细信息，请参阅[向 Azure AD 应用提供可选声明](/azure/active-directory/develop/active-directory-optional-claims)。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|idToken|[optionalClaim](optionalclaim.md) 集合| JWT ID 令牌中返回的可选声明。 |
|accessToken|[optionalClaim](optionalclaim.md) 集合| JWT 访问令牌中返回的可选声明。 |
|saml2Token|[optionalClaim](optionalclaim.md) 集合| SAML 令牌中返回的可选声明。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.optionalClaims"
}-->
``` json
{
  "idToken": [{"@odata.type": "microsoft.graph.optionalClaim"}],
  "accessToken": [{"@odata.type": "microsoft.graph.optionalClaim"}],
  "saml2Token": [{"@odata.type": "microsoft.graph.optionalClaim"}]
}
```
