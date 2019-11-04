---
title: optionalClaims 类型
description: 声明应用程序请求的可选声明。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 08481118457188ded581d494a745c4eb51b61edf
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37934272"
---
# <a name="optionalclaims-resource-type"></a>optionalClaims 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

声明应用程序请求的可选声明。 应用程序可以配置可从安全令牌服务接收的三种令牌（ID 令牌、访问令牌、SAML 2 令牌）每种类型中返回的可选声明。 应用程序可以配置要在每个令牌类型中返回的一组不同的可选声明。 [应用程序](application.md)的 optionalClaims 属性是一个**optionalClaims**对象。

应用程序开发人员可以在其 Azure AD 应用中配置可选声明，以在 Microsoft 安全令牌服务向其应用程序发送令牌中指定要使用的声明。 有关详细信息，请参阅向[AZURE AD 应用提供可选声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)。

## <a name="properties"></a>属性
| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|idToken|[optionalClaim](optionalclaim.md)集合| JWT ID 令牌中返回的可选声明。 |
|accessToken|[optionalClaim](optionalclaim.md)集合| JWT 访问令牌中返回的可选声明。 |
|saml2Token|[optionalClaim](optionalclaim.md)集合| SAML 令牌中返回的可选声明。|

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
