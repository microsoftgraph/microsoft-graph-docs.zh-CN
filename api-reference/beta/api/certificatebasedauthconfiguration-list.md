---
title: 列出 certificateBasedAuthConfigurations
description: 获取 certificatebasedauthconfiguration 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7452f081725dab0b98c7f45529bc9416018df2c3
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667622"
---
# <a name="list-certificatebasedauthconfigurations"></a>列出 certificateBasedAuthConfigurations

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取[certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md)对象的列表。

> [!NOTE]
> 集合中只能存在一个 certificateBasedAuthConfiguration 实例。 它始终具有值为 "29728ade-6ae4-4ee9-9103-412912537da5" 的固定 ID。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 全部, 全部组织。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序    | 全部, 全部组织。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfigurations"
}-->

```http
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration
```

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "certificateAuthorities": [
        {
          "isRootAuthority": true,
          "certificateRevocationListUrl": "CRLUrl-value",
          "deltaCertificateRevocationListUrl": "deltaCRLUrl-value",
          "certificate": "Binary",
          "issuer": "issuer-value",
          "issuerSki": "issuerSki-value"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->