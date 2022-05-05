---
title: channel： doesUserHaveAccess
description: 确定用户是否有权访问共享通道。
author: devjha-ms
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 808814a7c535a8a2ba9856eda0d8ec36a1170670
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211042"
---
# <a name="channel-doesuserhaveaccess"></a>channel： doesUserHaveAccess
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

确定 [用户](../resources/useridentity.md) 是否有权访问共享 [通道](../resources/channel.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户） | ChannelMember.Read.All、 ChannelMember.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | ChannelMember.Read.All、 ChannelMember.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/channels/{channel-id}/doesUserHaveAccess
```

## <a name="function-parameters"></a>函数参数
在请求 URL 中，提供以下查询参数（含值）。
下表显示了可用于此函数的参数。

|参数|类型|说明|
|:---|:---|:---|
|tenantId|字符串|[用户](../resources/useridentity.md)所属的Azure Active Directory租户的 ID。 此属性的默认值是已登录用户或应用的当前 **tenantId** 。|
|userId|字符串|[用户](../resources/useridentity.md)的唯一标识符。 在请求中指定 **userId** 或 **userPrincipalName** 属性。|
|userPrincipalName|String|用户的 UPN)  ([用户](../resources/useridentity.md)主体名称。 在请求中指定 **userId** 或 **userPrincipalName** 属性。|


## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿为此函数提供请求正文。

## <a name="response"></a>响应

如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 Boolean。

## <a name="examples"></a>示例

### <a name="example-1-check-access-for-an-internal-user"></a>示例 1：检查内部用户的访问权限

下面是检查内部用户是否有权访问共享通道的请求示例。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel_doesuserhaveaccess"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{0fddfdc5-f319-491f-a514-be1bc1bf9ddc}/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/doesUserHaveAccess(userId='6285581g-484b-4845-9e01-60667f8b12ae')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-doesuserhaveaccess-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-doesuserhaveaccess-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-doesuserhaveaccess-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-doesuserhaveaccess-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "@odata.type": "string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": true
}
```


### <a name="example-2-check-access-for-an-external-user"></a>示例 2：检查外部用户的访问权限

下面是使用 **tenantId** 属性检查外部用户是否有权访问共享通道的请求示例。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel_doesuserhaveaccess_externaluser"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{0fddfdc5-f319-491f-a514-be1bc1bf9ddc}/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/doesUserHaveAccess(userId='62855810-484b-4823-9e01-60667f8b12ae', tenantId='57fb72d0-d811-46f4-8947-305e6072eaa5')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-doesuserhaveaccess-externaluser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-doesuserhaveaccess-externaluser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-doesuserhaveaccess-externaluser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-doesuserhaveaccess-externaluser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "@odata.type": "string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": true
}
```


### <a name="example-3-check-user-access-for-a-user-using-the-user-principal-name"></a>示例 3：使用用户主体名称检查用户的访问权限

下面是使用 **userPrincipalName** 属性检查内部用户是否有权访问共享通道的请求示例。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel_doesuserhaveaccess_usingupn"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{0fddfdc5-f319-491f-a514-be1bc1bf9ddc}/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/doesUserHaveAccess(userPrincipalName='john.doe@contoso.com')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-doesuserhaveaccess-usingupn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-doesuserhaveaccess-usingupn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-doesuserhaveaccess-usingupn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-doesuserhaveaccess-usingupn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "@odata.type": "string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": false
}
```

