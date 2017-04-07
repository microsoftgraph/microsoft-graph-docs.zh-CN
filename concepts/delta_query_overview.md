#  <a name="use-delta-query-to-track-changes-in-microsoft-graph-data-preview"></a>使用增量查询跟踪 Microsoft Graph 数据更改（预览）

Delta 查询使应用程序能够发现新创建、更新或删除的实体，无需使用每个请求对目标资源执行完全读取。Microsoft Graph 应用程序可以使用 delta 查询和本地数据存储高效地同步更改。

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>使用 delta 查询来跟踪资源集合的更改

通常的调用模式如下：

1.  应用程序首先对所需资源运行 delta 函数以调用 GET 请求。
2.  Microsoft Graph 将发送一个包含已请求资源和[状态令牌](#state-tokens)的响应。

     a.如果返回了 `nextLink` URL，则会话中存在要检索的其他数据页面。应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。

     b.如果返回了 `deltaLink` URL，则未返回关于资源现有状态的更多数据。为了执行以后的请求，应用程序使用 `deltaLink` URL 了解资源更改。
     
3.  当应用程序需要了解资源更改时，会使用步骤 2 中收到的 `deltaLink` URL 发出新请求。*可能*在完成步骤 2 或应用程序检查更改时立即发出此请求。
4.  Microsoft Graph 返回响应，描述自上一个请求以来的资源更改和 `nextLink` URL 或 `deltaLink` URL。

### <a name="state-tokens"></a>状态令牌

增量查询 GET 响应中始终返回 `nextLink` 或 `deltaLink` 响应头中指定的 URL。`nextLink` URL 包含的是 _skipToken_，`deltaLink` URL 包含的是 _deltaToken_。 

这些令牌对客户端完全不透明。以下是需要了解的所有信息：

- 每个令牌都反映状态，并表示一轮更改跟踪中的响应快照。 
- 这些状态令牌还对初始增量查询请求中指定的其他查询参数（如 `$select`，如果资源支持的话）进行编码并将其包含在内，这样你就不必在后续增量查询请求中重复操作了。
- 执行增量查询时，只需将 `nextLink` 或 `deltaLink` URL 原样复制并应用到下一个 **delta** 函数调用即可，无需检查 URL 的内容（包括其状态令牌）。


### <a name="optional-query-parameters"></a>可选的查询参数

如果客户使用查询参数，则它必须在初始请求中指定。Microsoft Graph 自动将指定参数编码为响应中提供的 `nextLink` 或 `deltaLink`。调用应用程序只需预先指定其所需的查询参数一次。Microsoft Graph 将为所有后续请求自动添加指定参数。

对于用户和组，在使用某些查询参数时受到限制：

-   如果使用的是 `$select` 查询参数，则表示客户倾向于仅跟踪 `$select` 语句中指定的属性或关系的更改。这意味着如果未选中的属性发生更改，则属性已更改的资源将不会出现在后续请求之后的 delta 响应中。
-   不支持 `$expand`。

## <a name="resource-representation-in-the-delta-query-response"></a>delta 查询响应中的资源表示形式

-   在 delta 查询响应中，使用标准表示形式表示受支持资源的新建实例。

-   更新实例由它们的 **id** 表示，*至少*具有已更新的属性，但可能也包含其他属性。

-   用户和组的关系更改被表示为对标准资源表示形式的注释。这些注释将使用 `propertyName@delta`格式，仅当客户使用 `$select` 参数显式选择跟踪关系更改时才会出现。

-   删除的实例仅使用其 **id** 和 `@removed` 节点表示。`@removed` 节点可能包含有关为何删除该实例的其他信息。

> **对以后更改的说明**：删除的实例的 `@removed` 节点当前以 *“@removed” : “reason for removal”* 的格式出现。但是，未来将会进行重大更改。在 delta 查询从 /beta 移动到 /v1.0 之前，将在删除的节点内嵌套一个对象，以提供更多信息。例如，*@removed {reason: “reason for removal”}*。此对象可以在以后展开，以包含有关此删除的其他元数据。

## <a name="supported-resources"></a>支持的资源

当前 delta 查询支持在 Microsoft Graph /beta 终结点上预览以下资源。

| **资源集合** | **API** |
|:------ | :------ |
| 主日历的日历视图（日期范围）中的事件 | [事件](../api-reference/beta/resources/event.md)资源的 [delta](../api-reference/beta/api/event_delta.md) 函数 |
| 组 | [组](../api-reference/beta/resources/group.md)资源的 [delta](../api-reference/beta/api/group_delta.md) 函数 |
| 邮件文件夹 | [邮件文件夹](../api-reference/beta/resources/mailFolder.md)资源的 [delta](../api-reference/beta/api/mailfolder_delta.md) 函数 |
| 文件夹中的邮件 | [邮件](../api-reference/beta/resources/message.md)资源的 [delta](../api-reference/beta/api/message_delta.md) 函数 | 
| 私人联系人文件夹 | [联系人文件夹](../api-reference/beta/resources/contactfolder.md)资源的 [delta](../api-reference/beta/api/contactfolder_delta.md) 函数 |
| 文件夹中的私人联系人 | [联系人](../api-reference/beta/resources/contact.md)资源的 [delta](../api-reference/beta/api/contact_delta.md) 函数 |
| 用户 | [用户](../api-reference/beta/resources/user.md)资源的 [delta](../api-reference/beta/api/user_delta.md) 函数 | 
| 驱动器项目\* | [driveItem](../api-reference/beta/resources/driveItem.md) 资源的 [delta](../api-reference/beta/api/item_delta.md) 函数 |


> \* v1.0 已支持跟踪对驱动器及其子级所做的更改。使用模式与其他支持资源类似，仅存在一些小的语法差异。以后将更新驱动器增量查询，以与其他资源类型保持一致。有关当前语法的详细信息，请访问 <https://developer.microsoft.com/zh-cn/graph/docs/api-reference/v1.0/api/item_delta>

## <a name="prerequisites"></a>先决条件

在对某个特定资源执行 delta 查询时也需要阅读该资源所需的相同[权限](../authorization/permission_scopes.md)。

## <a name="known-limitations"></a>已知限制

仅在跟踪其更改的特定资源类中才支持跟踪对用户和组的关系更改。例如，如果客户端正在跟踪*组*更改并且已选择**成员**关系，若这些成员也是*组*，则客户端将只接收 delta 查询响应中的成员身份更新。换句话说，就是尚不支持跟踪用户的组成员身份。Microsoft Graph 团队知道这是一个高优先级方案，且目标是要在 2017 年 3 月发布此更新。

## <a name="delta-query-request-examples"></a>Delta 查询请求示例 

- [获取日历视图中事件的增量更改（预览）](../Concepts/delta_query_events.md)
- [获取文件夹中邮件的增量更改（预览）](./delta_query_messages.md)
- [获取组的增量更改（预览）](./delta_query_groups.md)
- [获取用户的增量更改（预览）](./delta_query_users.md)