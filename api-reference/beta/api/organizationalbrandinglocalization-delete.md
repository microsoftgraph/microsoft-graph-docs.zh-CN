---
title: 删除 organizationalBrandingLocalization
description: 删除 organizationalBrandingLocalization 对象。
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 883f441cd2726abd4e496d7d63b4b3a6d07da8c1
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777368"
---
# <a name="delete-organizationalbrandinglocalization"></a>删除 organizationalBrandingLocalization
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除本地化的品牌对象。 若要删除 [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) 对象， (Stream 类型) 必须先从该对象中删除。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Organization.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /organization/{organizationId}/branding/localizations/{organizationalBrandingLocalizationId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面是一个请求删除本地化对象 `fr-FR` 的示例。

<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandinglocalization"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR
```


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

