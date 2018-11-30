---
title: 获取 governanceResource
description: 检索的属性和 governanceResource 对象的关系。
ms.openlocfilehash: d871dbe91b82cebc01a8c282c0afdfbd8701c8f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041925"
---
# <a name="get-governanceresource"></a>获取 governanceResource

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

检索的属性和[governanceResource](../resources/governanceresource.md)对象的关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureResources  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | PrivilegedAccess.ReadWrite.AzureResources |

除了权限范围，此 API 要求具有至少一个角色分配对资源的请求程序。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法**仅**支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应正文中的响应代码和[governanceResource](../resources/governanceresource.md)对象。

## <a name="example"></a>示例
本示例演示如何获取订阅 Wingtip Toys-prod 移 (e5e7d29d-5465-45ac-885f-4716a5ee74b5) 的详细信息。
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a>请求
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 459

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources/$entity",
    "id": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",
    "type": "subscription",
    "displayName": "Wingtip Toys - Prod",
    "status": "Active",
    "onboardDateTime": "2018-04-05T22:30:37.13Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
