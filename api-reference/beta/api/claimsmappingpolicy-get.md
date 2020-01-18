---
title: 获取 claimsMappingPolicy
description: 检索 claimsMappingPolicy 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 80a9fd1a9f32fa7c0a5bfcf2a48bb1fc267c39b2
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234157"
---
# <a name="get-claimsmappingpolicy"></a>获取 claimsMappingPolicy

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的属性和关系。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Policy.Read.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | Policy.Read.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持`$expand`和`$select` OData 查询参数来帮助自定义响应。 有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。 使用`$expand`时，请确保您的应用程序请求读取扩展的对象的权限。

## <a name="request-headers"></a>请求头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/policies/claimsMappingPolicies/{id}
```

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->