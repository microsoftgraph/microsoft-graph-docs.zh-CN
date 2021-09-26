---
title: 删除 organizationalBrandingLocalization
description: 删除 organizationalBrandingLocalization 对象。
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 62df5020c5fb29a2e8987fbc25ec11fd1a5684ee
ms.sourcegitcommit: 7ce66321abb6a2cdca8685d3ce0a004c376ae33b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59778020"
---
# <a name="delete-organizationalbrandinglocalization"></a>删除 organizationalBrandingLocalization
命名空间：microsoft.graph

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
DELETE https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR
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

