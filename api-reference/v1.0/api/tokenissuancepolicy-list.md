---
title: 列出 tokenIssuancePolicy
description: 获取 tokenIssuancePolicy 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 32242e6ad6f6285ba04df02688623a100224d818
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229673"
---
# <a name="list-tokenissuancepolicy"></a>列出 tokenIssuancePolicy

命名空间：microsoft.graph



获取[tokenIssuancePolicy](../resources/tokenIssuancePolicy.md)对象的列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Policy： Read. All，ApplicationConfiguration |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | Policy： Read. All，ApplicationConfiguration |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenIssuancePolicies
```

## <a name="optional-query-parameters"></a>可选的查询参数

`$expand`此方法支持`$filter`、、 `$select`和`$top` OData 查询参数来帮助自定义响应。 有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。 使用`$expand`时，请确保您的应用程序请求读取展开的对象的权限。

## <a name="request-headers"></a>请求头

| 名称      |说明|
|:----------|:----------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和[tokenIssuancePolicy](../resources/tokenIssuancePolicy.md)对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "tokenIssuancePolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies
```

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
