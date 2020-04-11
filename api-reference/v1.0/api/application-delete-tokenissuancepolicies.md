---
title: 删除 tokenIssuancePolicy
description: 从应用程序中删除 tokenIssuancePolicy。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 670a5cb10c8209ed6e30a5cb8115b752f398487c
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227796"
---
# <a name="remove-tokenissuancepolicy"></a>删除 tokenIssuancePolicy

命名空间：microsoft.graph



从[应用程序](../resources/application.md)中删除[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) 。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenIssuancePolicies/{id}/$ref
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/tokenIssuancePolicies/{id}/$ref
```

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
