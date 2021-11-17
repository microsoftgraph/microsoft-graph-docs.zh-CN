---
title: 列出订阅
description: " 有关详细信息，请参阅下面的方案。"
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: eaab61771feca5c5e1f900295509da5460c1e52d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002070"
---
# <a name="list-subscriptions"></a>列出订阅

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 webhook 订阅列表。 响应的内容取决于应用调用的上下文;有关详细信息，请参阅下面的方案。

## <a name="permissions"></a>权限

此 API 支持以下权限范围；要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型  | 权限（从最低特权到最高特权）  |
|:---------------- |:-------------------------------------------- |
| [委派 (](/graph/auth-v2-user) 工作或学校帐户)  | 创建订阅 [或](subscription-post-subscriptions.md) Subscription.Read.All (请参阅下面的) 。 |
| [委派 (](/graph/auth-v2-user) 个人 Microsoft 帐户)  | 创建订阅 [或](subscription-post-subscriptions.md) Subscription.Read.All (请参阅下面的) 。 |
| [应用程序](/graph/auth-v2-service) | 创建订阅 [所需的权限](subscription-post-subscriptions.md)。 |

响应结果基于调用应用的上下文。 以下是常见方案的摘要：

### <a name="basic-scenarios"></a>基本方案

最常见的情况是，应用程序希望检索最初为当前登录用户或者检索目录中的所有用户（工作/学校帐户）创建的订阅。 除了应用最初用于创建订阅的权限外，这些方案不需要任何特殊权限。

| 调用应用程序的上下文 | 响应包含 |
|:-----|:---------------- |
| 应用程序代表已登录用户（委派权限）进行调用。 <br/>-且-<br/>应用程序具有[创建该订阅](subscription-post-subscriptions.md)所需的初始权限。<br/><br/>注意：这适用于个人 Microsoft 帐户和工作/学校帐户。 | **此应用** 仅为登录用户创建的订阅。 |
| 应用程序代表本身（应用程序权限）进行调用。<br/>-且-<br/>应用程序具有[创建该订阅](subscription-post-subscriptions.md)所需的初始权限。<br/><br/>注意：这仅适用于工作/学校帐户。| **此应用** 仅为自己或者目录中的任何用户创建的订阅。|

### <a name="advanced-scenarios"></a>高级方案

在某些情况下，应用想要检索其他应用创建的订阅。 例如，用户希望看到任何应用程序代表他们创建的所有订阅。 或者，管理员可能希望查看其目录中所有应用的所有订阅。
对于此类方案，委派权限 Subscription.Read.All 是必需的。

| 调用应用程序的上下文 | 响应包含 |
|:-----|:---------------- |
| 应用程序代表已登录用户（委派权限）进行调用。 *用户是非管理员*。 <br/>-且-<br/>应用程序具有权限 Subscription.Read.All<br/><br/>注意：这适用于个人 Microsoft 帐户和工作/学校帐户。 | **任何应用** 仅为登录用户创建的订阅。 |
| 应用程序代表已登录用户（委派权限）进行调用。 *用户是管理员*。<br/>-且-<br/>应用程序具有权限 Subscription.Read.All<br/><br/>注意：这仅适用于工作/学校帐户。 | **任何应用** 为目录中的 **任何用户** 创建的订阅。|

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法不支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象列表。

## <a name="example"></a>示例

##### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-subscriptions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应

下面是一个响应示例。 注意：为简洁起见，可能会截断此处显示的响应。 所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
      "latestSupportedTlsVersion": "v1_2",
      "encryptionCertificate": "",
      "encryptionCertificateId": "",
      "includeResourceData": false,
      "notificationContentType": "application/json"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

> **注意：** 出于安全目的，不会返回 `clientState` 属性值。  

当请求返回多页数据时，响应中包含一个 `@odata.nextLink` 属性，可帮助你管理结果。  若要了解详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。
