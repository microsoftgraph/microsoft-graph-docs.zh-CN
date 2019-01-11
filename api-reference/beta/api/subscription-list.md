---
title: 列表订阅
description: " 请参阅下面的方案的详细信息。"
localization_priority: Normal
ms.openlocfilehash: 1b751b8632d82626e2ba87bf00a054b2be4f25f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876984"
---
# <a name="list-subscriptions"></a>列表订阅

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

检索 webhook 订阅的列表。 将响应的内容取决于的上下文中调用应用程序;请参阅下面的方案的详细信息。

## <a name="permissions"></a>Permissions

此 API 支持以下权限范围;若要了解详细信息，包括如何选择权限，请参阅[权限](/graph/permissions-reference)。

| 权限类型  | 权限（从最低特权到最高特权）  |
|:---------------- |:-------------------------------------------- |
| [委派](/graph/auth-v2-user)（工作或学校帐户） | [创建订阅](subscription-post-subscriptions.md)或 Subscription.Read.All （见下文） 所需的权限。 |
| [委派](/graph/auth-v2-user)（个人 Microsoft 帐户） | [创建订阅](subscription-post-subscriptions.md)或 Subscription.Read.All （见下文） 所需的权限。 |
| [Application](/graph/auth-v2-service) | [创建订阅](subscription-post-subscriptions.md)所需的权限。 |

响应结果基于调用应用程序的上下文。 以下是常见方案的摘要：

### <a name="basic-scenarios"></a>基本方案

大多数情况下，应用程序要检索其最初创建对当前已登录的用户或 （工作/学校帐户） 的目录中的所有用户的订阅。 这些方案不需要之外的任何特殊权限最初用于创建其订阅应用程序。

| 调用应用程序的上下文 | 响应中包含 |
|:-----|:---------------- |
| 应用程序代表登录用户 （委派权限） 调用。 <br/>-和-<br/>应用程序具有到[创建订阅，](subscription-post-subscriptions.md)所需的原始权限。<br/><br/>注意： 这适用于个人 Microsoft 帐户和工作/学校帐户。 | 创建的**此应用程序**的已登录的用户的订阅。 |
| 应用程序调用代表本身 （应用程序的权限）。<br/>-和-<br/>应用程序具有到[创建订阅，](subscription-post-subscriptions.md)所需的原始权限。<br/><br/>注意： 这适用于工作/学校仅帐户。| 创建**此**应用程序本身或目录中的任何用户的订阅。|

### <a name="advanced-scenarios"></a>高级的方案

在某些情况下，希望检索订阅创建其他应用程序的应用程序。 例如，用户想要查看由其代表任何应用程序创建的所有订阅。 或者，管理员可能希望查看其目录中的所有应用程序中的所有订阅。
如果是这种情况下，对于需要委派的权限 Subscription.Read.All。

| 调用应用程序的上下文 | 响应中包含 |
|:-----|:---------------- |
| 应用程序代表登录用户 （委派权限） 调用。 *用户在处于非管理员*。 <br/>-和-<br/>应用程序具有权限 Subscription.Read.All<br/><br/>注意： 这适用于个人 Microsoft 帐户和工作/学校帐户。 | 创建的**任何应用程序**的已登录的用户的订阅。 |
| 应用程序代表登录用户 （委派权限） 调用。 *用户是管理员*。<br/>-和-<br/>应用程序具有权限 Subscription.Read.All<br/><br/>注意： 这适用于工作/学校仅帐户。 | 创建的**任何应用程序**目录中的**任何用户**的订阅。|

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法不支持的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)以帮助自定义的响应。

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应代码和响应正文中的[订阅](../resources/subscription.md)对象的列表。

## <a name="example"></a>示例

##### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a>响应

下面是一个响应示例。 注意： 为了简单起见，如下所示的响应可能被截断。 将从实际调用中返回所有属性。

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 586

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
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

请求返回的数据的多个页面，响应中包括`@odata.nextLink`属性可帮助您管理结果。  若要了解详细信息，请参阅[分页 Microsoft Graph 应用程序中的数据](/graph/paging)。
