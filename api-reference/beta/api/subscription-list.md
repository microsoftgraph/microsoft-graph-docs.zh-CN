---
title: 列出订阅
description: " 有关详细信息, 请参阅以下方案。"
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 20aad712bc49f91bec58a67c0c66ef76bf4653e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537088"
---
# <a name="list-subscriptions"></a>列出订阅

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 webhook 订阅的列表。 响应的内容取决于在其中调用应用程序的上下文。有关详细信息, 请参阅以下方案。

## <a name="permissions"></a>权限

此 API 支持以下权限范围;若要了解详细信息, 包括如何选择权限, 请参阅[权限](/graph/permissions-reference)。

| 权限类型  | 权限（从最低特权到最高特权）  |
|:---------------- |:-------------------------------------------- |
| [委派](/graph/auth-v2-user)(工作或学校帐户) | [创建订阅](subscription-post-subscriptions.md)或订阅所需的权限。 Read. 所有 (请参阅下面的)。 |
| [委派](/graph/auth-v2-user)(个人 Microsoft 帐户) | [创建订阅](subscription-post-subscriptions.md)或订阅所需的权限。 Read. 所有 (请参阅下面的)。 |
| [应用程序](/graph/auth-v2-service) | [创建订阅](subscription-post-subscriptions.md)所需的权限。 |

响应结果基于呼叫应用程序的上下文。 以下是常见方案的摘要:

### <a name="basic-scenarios"></a>基本方案

通常情况下, 应用程序希望检索它最初为当前登录用户创建的订阅, 或者检索目录 (工作/学校帐户) 中的所有用户。 这些方案不需要除了最初用于创建订阅的应用程序之外的任何特殊权限。

| 呼叫应用程序的上下文 | 响应包含 |
|:-----|:---------------- |
| 应用代表已登录用户 (委派权限) 呼叫。 <br/>并<br/>应用程序具有[创建订阅](subscription-post-subscriptions.md)所需的原始权限。<br/><br/>注意: 这适用于个人 Microsoft 帐户和工作/学校帐户。 | 仅**此应用**为登录用户创建的订阅。 |
| 应用程序是代表自身调用的 (应用程序权限)。<br/>并<br/>应用程序具有[创建订阅](subscription-post-subscriptions.md)所需的原始权限。<br/><br/>注意: 这仅适用于工作/学校帐户。| **此应用**为自己或目录中的任何用户创建的订阅。|

### <a name="advanced-scenarios"></a>高级方案

在某些情况下, 应用想要检索由其他应用程序创建的订阅。 例如, 用户希望以代表自己的任意方式查看由任何应用程序创建的所有订阅。 或者, 管理员可能想要查看其目录中所有应用程序的所有订阅。
在这种情况下, 委派权限订阅是必需的。 All 是必需的。

| 呼叫应用程序的上下文 | 响应包含 |
|:-----|:---------------- |
| 应用代表已登录用户 (委派权限) 呼叫。 *用户是非管理员*。 <br/>并<br/>应用具有权限订阅。 Read. All<br/><br/>注意: 这适用于个人 Microsoft 帐户和工作/学校帐户。 | 仅供登录用户使用的**任何应用程序所**创建的订阅。 |
| 应用代表已登录用户 (委派权限) 呼叫。 *用户是管理员*。<br/>并<br/>应用具有权限订阅。 Read. All<br/><br/>注意: 这仅适用于工作/学校帐户。 | 由目录中**任何用户**的**任何应用程序**创建的订阅。|

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法不支持[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和[订阅](../resources/subscription.md)对象列表。

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

下面是一个响应示例。 注意: 为简洁起见, 可能会截断此处显示的响应。 所有属性都将通过实际调用返回。

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
<!--
{
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

当请求返回多个数据页时, 响应中包含一个`@odata.nextLink`可帮助您管理结果的属性。  若要了解详细信息, 请参阅[在应用中分页 Microsoft Graph 数据](/graph/paging)。
