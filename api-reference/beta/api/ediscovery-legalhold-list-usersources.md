---
title: 列出 legalHold userSources
description: 从 userSources 导航属性获取 userSource 资源。
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 58d4f2019f403659cbd46f3a462acbcd653fafc2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986759"
---
# <a name="list-legalhold-usersources"></a>列出 legalHold userSources

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取与 [合法保留相关联的 userSource](../resources/ediscovery-usersource.md) 对象列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|eDiscovery.Read.All、eDiscovery.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/userSources
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/277107ff-fee3-41a0-a665-a9d7f6c4824f/userSources
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usersource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usersource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usersource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usersource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-usersource-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.userSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('c816dd6f-5af8-40c5-a760-331361e05c60')/legalholds('277107ff-fee3-41a0-a665-a9d7f6c4824f')/userSources",
    "value": [
        {
            "displayName": "Adele Vance",
            "createdDateTime": "2020-10-30T21:02:41.887Z",
            "id": "2f279b24-2142-435d-97c5-0d42220ba453",
            "email": "AdeleV@contoso.com",
            "includedSources": "mailbox",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "eDiscovery admin"
                }
            }
        }
    ]
}
```
