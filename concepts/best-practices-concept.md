---
title: 使用 Microsoft Graph 的最佳做法
description: 本文介绍可用于帮助你的应用程序充分利用 Microsoft Graph 的最佳做法，内容涉及了解 Microsoft Graph、提高应用性能，以及让应用程序对最终用户更具可靠性等。
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 97e07faac83e1d25dfc133fdda7484397b51ef71b1f8e385e027579fd8209c90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149588"
---
# <a name="best-practices-for-working-with-microsoft-graph"></a>使用 Microsoft Graph 的最佳做法

本文介绍可用于帮助你的应用程序充分利用 Microsoft Graph 的最佳做法，内容涉及了解 Microsoft Graph、提高应用性能，以及让应用程序对最终用户更具可靠性等。

## <a name="use-graph-explorer-to-get-to-know-the-api"></a>使用 Graph 浏览器了解 API

开始探索可通过 Microsoft Graph 提供的数据的最简便方法是使用 [Graph 浏览器](https://aka.ms/ge)。 通过 Graph 浏览器，你可以手动编写 REST 请求（带有完整的 CRUD 支持）、调整 HTTP 请求头，以及查看数据响应。 为了帮助你入门，Graph 浏览器还提供了一组查询示例。

在将它们集成到应用程序之前，请尝试使用新的 API。

## <a name="authentication"></a>身份验证

要访问 Microsoft Graph 中的数据，应用程序需要获得一个 OAuth 2.0 访问令牌，并通过以下任一方式将其呈现给 Microsoft Graph：

- HTTP *授权* 请求头（作为一个 *持有者* 令牌）
- Graph 客户端构造函数（当使用 Microsoft Graph 客户端库时）

使用 Microsoft 身份验证库 API ([MSAL](/azure/active-directory/develop/active-directory-v2-libraries)) 来获得 Microsoft Graph 的访问令牌。

## <a name="consent-and-authorization"></a>许可和授权

在应用中适用以下面向许可和授权的最佳做法：

- **使用最小特权**。 只请求绝对必要的权限，并且只在需要时请求。 对于应用程序调用的 API，查看方法主题中的权限部分（例如，查看[创建用户](/graph/api/user-post-users)），然后选择最小特权权限。 有关权限的完整列表，请参阅[权限引用](permissions-reference.md)。

- **根据应用场景使用正确的权限类型**。 如果你正在构建交互式应用程序，其中存在一个已登录用户，那么应用程序应使用 *委派* 权限，在此权限中，应用程序被授权在调用 Microsoft Graph 时充当已登录用户。 但是，如果应用程序在没有已登录用户的情况下运行（如后台服务或守护程序），那么应用程序应使用应用程序权限。

    >**注意：** 将应用程序权限用于交互式场景会将你的应用程序置于合规性与安全性风险中。 它可能会不小心提升用户权限来访问数据，绕过管理员配置的策略。
<!-- LG: Use a more clear lead-in here, like "Consider the end user and admin experience"? -->
- **在配置应用时请考虑周全**。 这会直接影响最终用户和管理体验，以及应用程序的采用和安全性。 例如：

  - 应用程序的隐私声明、使用条款、名称、徽标和域名都将出现在同意和其他体验中，所以一定要仔细配置，以便终端用户可以理解它们。
  - 考虑谁将同意你的应用程序（终端用户或管理员），并适当将应用程序配置为[请求权限](/azure/active-directory/develop/active-directory-v2-scopes)。
  - 确保理解[静态、动态和增量同意](/azure/active-directory/develop/active-directory-v2-compare#incremental-and-dynamic-consent)之间的区别。

- **请考虑多租户应用程序**。 预期客户有不同的应用程序和不同状态的同意控件。 例如：

  - 租户管理员可以禁用最终用户同意应用程序的功能。 在这种情况下，管理员需要代表他们的用户同意。
  - 租户管理员可以设置自定义授权策略，如阻止用户读取其他用户的配置文件，或者将自助服务组创建限制为一组有限用户。 在这种情况下，应用程序应在代表用户操作的情况下处理 403 错误响应。

## <a name="handle-responses-effectively"></a>有效处理响应

根据你对 Microsoft Graph 发出的请求，应用程序应准备好处理不同类型的响应。 下面是一些要遵循的最为重要的做法，可确保应用程序能够可靠且可预测地为最终用户运行。

### <a name="pagination"></a>分页

当查询资源集合时，应料到 Microsoft Graph 会在多个页面中返回结果集，这是由于服务器端页面大小限制所致。 当结果集跨多个页面时，Microsoft Graph 将在响应中返回 `@odata.nextLink` 属性，其中包含指向结果下一页的 URL。

例如，列出已登录用户邮件：

```http
GET https://graph.microsoft.com/v1.0/me/messages
```

如果结果集超过服务器端页面大小限制，将返回包含 `@odata.nextLink` 属性的响应。

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$skip=23"
```

>**注意：** 应用程序应 **始终** 处理在本质上对响应进行分页的可能性，并使用 `@odata.nextLink` 属性获得下一个分页结果集，直到读取结果集的所有页面。 最后一页将不包含 `@odata.nextLink` 属性。 你应在请求的 `@odata:nextLink` 属性中包括整个 URL，以获取下一页结果，将整个 URL 视为一个不透明的字符串。

有关详细信息，请参阅[分页](paging.md)。

### <a name="handling-expected-errors"></a>处理预期错误

虽然应用程序应处理所有错误响应（在 400 和 500 范围内），但要特别注意某些预期的错误和响应，如下表所示。

| 主题   | HTTP 错误代码    | 最佳做法|
|:-----------|:--------|:----------|
| 用户无法访问 | 403 | 如果应用程序启动并运行，它可能会遇到此错误，即使它已经通过同意体验获得了必要的权限。  在这种情况下，最有可能的原因是登录用户没有权限访问所请求的资源。 应用程序应向登录用户反馈通用的“拒绝访问”错误。 |
|未找到| 404 | 在某些情况下，可能无法找到请求的资源。 例如，资源可能不存在，因为尚未预配（如用户照片），或者因为已被删除。 一些已删除的资源 *可能* 在删除后的 30 天内完全恢复（如用户、组和应用程序资源），因此，应用程序也应该考虑到这一点。|
|限制|429|由于各种原因，API 可能会随时受限，因此，应用程序必须 **始终** 准备好处理 429 响应。 此错误响应包括 HTTP 响应头中的“重试后”字段。 使用“重试后”延迟退出请求是从限制中恢复的最快方法。 有关详细信息，请参阅[限制](throttling.md)。|
|服务不可用| 503 | 这可能是因为服务繁忙。 应部署类似于 429 的退出策略。 此外，应 **始终** 通过新 HTTP 连接发出新的重试请求。|

### <a name="handling-future-members-in-evolvable-enumerations"></a>处理可演化枚举中的未来成员

在现有的枚举中添加成员会破坏已在使用这些枚举的应用程序。 可演化枚举是 Microsoft Graph API 用来向现有枚举添加新成员的机制，而不会对应用程序造成破坏性改变。

可演化的枚举具有一个名为 `unknownFutureValue` 的常见 _Sentinel_ 成员，其划分了最初在枚举中已定义的已知成员和随后添加的或将来要定义的未知成员。 在内部，将已知成员映射为小于 sentinel 成员的数值，而未知成员则大于 sentinel 成员。 可演化枚举的文档按照升序列出了可能的 _字符串_ 值: 已知成员，其次是 `unknownFutureValue`，其次是未知成员。 与其他类型的枚举一样，应 _始终_ 通过其 _字符串_ 值引用可演化枚举的成员。

默认情况下，GET 操作仅返回可演化枚举类型属性的已知成员，应用程序只需要处理已知成员。 如果设计的应用程序也能处理未知成员，则可以通过使用 HTTP `Prefer` 请求标头来选择接收这些成员:
```
Prefer: include-unknown-enum-members
```


## <a name="storing-data-locally"></a>在本地存储数据

理想情况下，应用程序应调用 Microsoft Graph 来根据需要实时检索数据。 仅当特定方案需要，并且该用例在使用条款和隐私策略的涵盖范围内，且不违反 [Microsoft API 使用条款](/legal/microsoft-apis/terms-of-use?context=/graph/context) 时，才能在本地缓存或存储数据。 应用程序还应该实现适当的保留和删除策略。

## <a name="optimizations"></a>优化

一般来说，出于性能甚至是安全或隐私方面的原因，应只获取应用程序真正需要的数据，仅此足矣。

### <a name="use-projections"></a>使用投影

只选择应用程序真正需要的属性，仅此即可，因为这样可以在应用程序（和服务中）节省不必要的网络流量和数据处理。

>**注意：** 使用 `$select` 查询参数将查询返回的属性限制为那些应用程序所需的属性。

例如，检索登录用户的邮件时，可以指定仅返回 **from** 和 **subject** 属性：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

### <a name="getting-minimal-responses"></a>获取最少响应

对于某些操作，如 PUT 和 PATCH（在某些情况下还包括 POST），如果应用程序不需要使用响应有效负载，则可以要求 API 返回最小数据。 请注意，有些服务已向 PUT 和 PATCH 操作返回 204 无内容响应。

>**注意：** 在适当情况下，使用 HTTP 请求头请求最小表示形式的响应：*首选：返回=最小*。 请注意，对于创建操作来说，这可能不合适，因为应用程序可能期望在响应中获得新建对象的服务生成 `id`。

### <a name="track-changes-delta-query-and-webhook-notifications"></a>跟踪更改：增量查询和 webhook 通知

如果应用程序需要了解数据变化，只要你所感兴趣的数据发生更改，就会获得 webhook 通知。 这比简单地定期轮询更为有效。

使用 [webhook 通知](/graph/api/resources/webhooks)，在数据发生变化时获得推送通知。

如果应用程序需要在本地缓存或存储 Microsoft Graph 数据，并使这些数据保持最新，或者出于其他原因需要跟踪数据变化，则应使用增量查询。 这样可以避免应用程序过度计算，以检索应用程序已有的数据，并最小化网络流量和降低达到限制阈值的可能性。

使用[增量查询](delta-query-overview.md)以有效保持数据最新。

### <a name="using-webhooks-and-delta-query-together"></a>结合使用 webhook 和增量查询

webhook 和增量查询通常结合使用效果更佳，因为如果单独使用增量查询，则需要找出正确的轮询间隔，间隔过短可能会导致空响应进而浪费资源，而间隔过长可能最终会获得陈旧数据。如果使用 webhook 通知作为触发器来进行 delta 查询调用，则能得到两方面的好处。

使用 [webhook 通知](/graph/api/resources/webhooks)作为触发器以触发增量查询调用。 此外，还应确保应用程序有一个支持轮询阈值，以防触发通知。

### <a name="batching"></a>批处理

JSON 批处理使你能够通过将多个请求合并为一个单一 JSON 对象优化应用程序。 将各个请求合并到一个单独的批请求中，可以使应用程序不受严重网络延迟的影响，并且可以节省连接资源。

使用[批处理](json-batching.md)时，严重的网络延迟会对性能产生很大的影响。

## <a name="reliability-and-support"></a>可靠性和支持
若要确保可靠性并为应用程序提供支持：

- 接受 DNS TTL 并设置连接 TTL 以进行匹配。 这可确保在故障转移情况下的可用性。
- 打开到所有播发 DNS 答案的连接。
- 生成唯一的 GUID 并随每个 Microsoft Graph REST 请求发送。 如果需要报告 Microsoft Graph 的问题，那么这将有助于 Microsoft 更轻松地调查任何错误。
  - 每次向 Microsoft Graph 发出请求时，会生成唯一的 GUID，将其随 `client-request-id` HTTP 请求标头发送，并将其记录在应用程序日志中。
  - 始终记录 HTTP 响应标头中的 `request-id`、`timestamp` 和 `x-ms-ags-diagnostic`。 在 [Microsoft Q&A](/answers/products/m365#microsoft-graph) 中或向 Microsoft 支持部门报告问题时，需要上述这些以及 `client-request-id`。
