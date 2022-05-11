---
title: 获取 connectionQuota
description: 检索 connectionQuota 的属性和关系。
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: a4b231af17d8fb60dd0a565da0ced57487dfa006
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315488"
---
# <a name="get-connectionquota"></a>获取 connectionQuota

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [connectionQuota](../resources/externalconnectors-connectionquota.md) 对象的属性和关系。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | ExternalConnection.ReadWrite.OwnedBy |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/quota
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持所有 [OData 查询参数](/graph/query-parameters) ，以帮助自定义响应。

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [externalConnection](../resources/externalconnectors-externalconnection.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "get_connection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/quota
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a>响应
<!-- markdownlint-enable MD024 -->

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.connectionQuota"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "itemsRemaining": 7000
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-12-02 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connectionQuota",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
