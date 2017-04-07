# <a name="working-with-webhooks-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Webhooks

Microsoft Graph REST API 使用 Webhook 机制来将通知传递到客户端。客户端是用于配置自身的 URL 以接收通知的 Web 服务。客户端应用使用通知在更改时更新其状态。

使用 Microsoft Graph REST API，应用可以订阅以下资源的更改：

* 邮件
* 事件
* 联系人
* 群组对话
* 驱动器根项

Microsoft Graph 接受订阅请求之后，它将通知推送到订阅中指定的 URL。然后应用程序根据其业务逻辑执行操作。例如，它获取更多数据，更新缓存和视图等。

应用应在过期之前续订其订阅。它们还可以随时取消订阅以停止获取通知。

在 GitHub 上查看以下代码示例。

* [Microsoft Graph Webhooks Sample for Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)（面向 Node.js 的 Microsoft Graph Webhooks 示例）
* [Microsoft Graph Webhooks Sample for ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)（面向 ASP.NET 的 Microsoft Graph Webhooks 示例）

我们来看一看订阅流程。

# <a name="creating-a-subscription"></a>创建订阅

创建订阅是开始接收资源通知的第一步。订阅流程如下所示：

1. 客户端发送特定资源的订阅 (POST) 请求。
2. Microsoft Graph 验证请求。
  * 如果请求有效，Microsoft Graph 将验证令牌发送到通知 URL。
  * 如果该请求无效，Microsoft Graph 将发送包含代码和详细信息的错误响应。
3. 客户端将验证令牌发送回 Microsoft Graph。

客户端必须存储订阅 ID 以便将通知与相应订阅关联。

## <a name="characteristics-of-subscriptions"></a>订阅的特征

可以创建这些资源的订阅，例如邮件、事件、联系人和驱动器根项。

可以创建特定文件夹的订阅：`https://graph.microsoft.com/v1.0/me/mailfolders('inbox')/messages`

或顶级资源的订阅：`https://graph.microsoft.com/v1.0/me/messages`

或驱动器根项的订阅：`https://graph.microsoft.com/v1.0/me/drive/root`

在大多数情况下，创建订阅都需要读取资源范围。例如，若要获取通知消息，应用程序需要 `mail.read` 权限。请注意，目前，OneDrive 驱动器根项需要 `Files.ReadWrite` 权限，与 SharePoint 站点关联的驱动器需要 `Files.ReadWrite.All` 权限。

订阅过期。当前的最长过期时间为，将三天减去从创建时起的 90 分钟（共计 4230 分钟）。需要在过期时间之前续订应用订阅。否则，它们将需要新建订阅。

## <a name="notification-url-validation"></a>通知 URL 验证

Microsoft Graph 在创建订阅之前验证订阅请求中的通知 URL。验证流程如下所示：

1. Microsoft Graph 将 POST 请求发送到通知 URL：

  ```
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```
 
2. 客户端必须在 10 秒内提供具有以下特性的响应：

  * 200 (OK) 状态代码。
  * 内容类型必须是 text/plain。 
  * 正文必须包括 Microsoft Graph 提供的验证令牌。

在响应中提供验证令牌之后，客户端应放弃验证令牌。

## <a name="subscription-request-example"></a>订阅请求示例

```
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

changeType、notificationUrl、resource 和 expirationDateTime 属性是必需的。如需属性定义和值，请参阅 [订阅资源类型](subscription.md)。虽然不需要 clientState，但必须包括它才能符合我们建议的通知处理过程。

如果成功，Microsoft Graph 在正文中返回 `200 OK` 代码和一个 [subscription](subscription.md) 对象。

# <a name="renewing-a-subscription"></a>续订订阅

客户端可以续订特定过期日期的订阅，自请求时间起长达三天。ExpirationDateTime 属性是必需的。

## <a name="subscription-renewal-example"></a>订阅续订示例

```
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

如果成功，Microsoft Graph 在正文中返回 `200 OK` 代码和一个 [subscription](subscription.md) 对象。订阅对象包括新的 expirationDateTime 值。 

# <a name="deleting-a-subscription"></a>删除订阅

客户端可以通过使用其 ID 删除订阅来停止接收通知。

```
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

如果成功，Microsoft Graph 将返回 `204 No Content` 代码。

# <a name="notifications"></a>通知

客户端在创建订阅后开始接收通知。资源发生更改时，Microsoft Graph 将 POST 请求发送到通知 URL。客户端只能根据指定的更改类型获取通知，例如 *created*。

## <a name="notification-properties"></a>通知属性

通知对象具有以下属性：

* id — 此通知所属的订阅的 ID。
* expirationDateTime — 订阅的过期时间。
* clientState — 订阅请求中指定的 clientState 属性。
* changeType — 引发通知的事件类型。例如，邮件接收时为 *created*，或将邮件标记为已读时为 *updated*。
* resource — 资源相对于 `https://graph.microsoft.com` 的 URI。 
* resourceData — 取决于订阅资源的对象。例如，对于 Outlook 资源：
  * @odata.type — Microsoft Graph 中描述所表示对象的 OData 实体类型。
  * @odata.id — 对象的 OData 标识符。
  * @odata.etag — 表示对象版本的 HTTP 实体标记。
  * Id — 对象的标识符。


> 注意：resourceData 中提供的 Id 值在通知已排入队列时有效。一些操作（例如将邮件移到其他文件夹中）可能会导致资源 Id 发生更改。 

## <a name="notification-example"></a>通知示例

用户收到电子邮件时，Microsoft Graph 将发送如下所示的通知：

```
{
  "value":[
  {
    "id":"<subscription_guid>",
    "expirationDateTime":"\"2016-03-19T22:11:09.952Z\"",
    "clientState":"SecretClientState",
    "changeType":"Created",
    "resource":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
    "resourceData":
    {
      "@odata.type":"#Microsoft.Graph.Message",
      "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
      "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
      "Id":"<long_id_string>"
    }
  }
  ]
}
```

请注意，值对象包含一个列表。如果有很多排队的通知，Microsoft Graph 在单个请求中发送它们。

## <a name="processing-the-notification"></a>处理通知

必须在应用程序开始接收通知后处理它们。应用程序必须至少执行以下任务来处理通知：

1. 验证 `clientState` 属性。通知中的 clientState 属性必须与订阅请求提交的属性匹配。
  > 注意：如果不符合这个条件，无需将其视为有效通知。还应调查通知来自何处并采取适当的措施。

2. 基于业务逻辑更新应用程序。
3. 将响应中的 `202 - Accepted` 状态代码发送到 Microsoft Graph。如果 Microsoft Graph 没有收到 2xx 类代码，它将重试多次发送通知。
  > 即使 clientState 属性与订阅请求提交的属性不匹配，也应发送 `202 - Accepted` 状态代码。

对请求中的其他通知重复该过程。

# <a name="additional-resources"></a>其他资源

* [订阅资源类型](subscription.md)
* [获取订阅](../api/subscription_get.md)
* [创建订阅](../api/subscription_post_subscriptions.md)
* [Microsoft Graph Webhooks Sample for Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)（面向 Node.js 的 Microsoft Graph Webhooks 示例）
* [Microsoft Graph Webhooks Sample for ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)（面向 ASP.NET 的 Microsoft Graph Webhooks 示例）
