# <a name="list-subscriptions"></a>订阅列表

基于应用程序ID、用户和用户与租户的角色，检索webhook订阅的属性和关系。

## <a name="permissions"></a>权限

此API支持以下权限范围；若要了解详细信息，包括如何选择权限，请参阅 [权限](../../../concepts/permissions_reference.md)。

| 权限类型  | 权限（从最低权限到最高特权）  |
|:---------------- |:-------------------------------------------- |
| [委派的](../../../concepts/auth_v2_user.md) （工作或学校帐户） |  [创建订阅](subscription_get.md) 或 Subscriptions.Read.All （见下文） 所需的角色。 |
| [委派的](../../../concepts/auth_v2_user.md) （个人 Microsoft 帐户） |  [创建订阅](./subscription_get.md) 或 Subscriptions.Read.All （见下文） 所需的角色。 |
| [应用程序](../../../concepts/auth_v2_service.md) | [创建订阅](./subscription_get.md)所需的角色。 |

响应结果基于调用应用程序的上下文。 以下是常见方案的总结：

### <a name="basic-scenarios"></a>基本方案

大多数情况下，应用程序要检索其最初创建对当前已登录的用户或目录中所有用户（工作/学校帐户）的订阅。 这些方案不需要最初用以创建其订阅的应用程序之外的任何特殊权限。

| 调用应用程序的上下文 | 响应中包含 |
|:-----|:---------------- |
| 应用程序代表登录用户调用（委派权限）。 <br/>-和-<br/>应用程序具有[创建订阅](subscription_post_subscriptions.md)所需的原始权限。<br/><br/>注意：这适用于个人 Microsoft 帐户和工作/学校帐户。 | 只为已登录用户创建的 **此应用程序** 的订阅。 |
| 应用程序调用代表本身 （应用程序的权限）。<br/>-和-<br/>应用程序具有[创建订阅](subscription_post_subscriptions.md)所需的原始权限。<br/><br/>注意：这只适用于工作/学校帐户。| 创建 **此应用程序** 本身或目录中任何用户的订阅。|

### <a name="advanced-scenarios"></a>高级方案

在某些情况下，应用程序希望检索其他应用程序创建的订阅。 例如，用户想要查看由任何应用程序代表其创建的所有订阅。 或者，管理员可能希望查看其目录中所有应用程序的所有订阅。
如果是这种情况下，需要委派权限 Subscription.Read.All。

| 调用应用程序的上下文 | 响应中包含 |
|:-----|:---------------- |
| 应用程序代表登录用户调用（委派权限）。 *用户非管理员*。 <br/>-和-<br/>应用程序具有 Subscription.Read.All 权限<br/><br/>注意： 这适用于个人 Microsoft 帐户和工作/学校帐户。 | 只为已登录用户创建的 **任何应用程序** 的订阅。 |
| 应用程序代表登录用户调用（委派权限）。 *用户是管理员*。<br/>-和-<br/>应用程序具有 Subscription.Read.All 权限<br/><br/>注意：这只适用于工作/学校帐户。 | 创建的 **任何应用程序** 目录中 **任何用户** 的订阅。|

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法不支持帮助适应于响应的 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 。

## <a name="request-headers"></a>请求的标头

| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| 授权  | 字符串  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [订阅](../resources/subscription.md) 对象列表。

## <a name="example"></a>示例

##### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a>响应

下面是响应的示例。  请注意，它可能会为了简便而被截断。  支持所有适用于请求的属性并从实际的调用返回调用上下文。

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions",
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

请求返回多个页面的数据时，响应中包括 `@odata.nextLink` 属性可帮助您管理结果。  若要了解详细信息，请参阅 [Paging Microsoft Graph 应用程序中的数据](../../../concepts/paging.md)。
