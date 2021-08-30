---
title: 获取 externalGroup
description: 获取 externalGroup 对象。
author: sacampbe-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 173118edbec82a9f594c5e6bccc1f9774a7ab19e
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697488"
---
# <a name="get-externalgroup"></a>获取 externalGroup
命名空间：microsoft.graph.externalConnectors


获取 [externalGroup](../resources/externalconnectors-externalgroup.md) 对象。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持                               |
| 委派（个人 Microsoft 帐户） | 不支持                               |
| 应用程序                            | ExternalItem.ReadWrite.OwnedBy、ExternalItem.ReadWrite.All|


## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /connections/{connectionsId}/groups/{externalGroupId}
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回包含 `200 OK` **externalGroup** 对象的 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_externalgroup"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/external/connections/contosohr/groups/31bea3d537902000
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
