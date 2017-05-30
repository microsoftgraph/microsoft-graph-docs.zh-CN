# <a name="known-issues-with-microsoft-graph"></a>Microsoft Graph 已知问题

本文介绍了 Microsoft Graph 的已知问题。有关最新更新的信息，请参阅 [ Microsoft Graph 更改日志](changelog.md)。

## <a name="users"></a>用户

### <a name="no-instant-access-after-creation"></a>创建后无法即时访问

可通过在用户实体上使用 POST 来即时创建用户。必须先向用户分配 Office 365 许可证，然后用户才能访问 Office 365 服务。尽管如此，由于服务具有分散特性，因此用户可能需要先等待 15 分钟，然后才能通过 Microsoft Graph API 使用文件、邮件和事件实体。在此期间，应用会收到一个 404 HTTP 错误响应。

### <a name="photo-restrictions"></a>照片限制

只有当用户有邮箱时，才能读取和更新用户的个人资料照片。另外，之前*可能*使用 **thumbnailPhoto** 属性（使用 Office 365 统一 API 预览或 Azure AD Graph，或通过 AD Connect 同步）存储的所有照片无法再通过[用户](../api-reference/v1.0/resources/user.md)资源的 Microsoft Graph **照片**属性进行访问。在这种情况下，无法读取或更新照片会生成以下错误：

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a>在用户邮箱中添加和访问基于 ICS 的日历

目前，还有部分支持基于 Internet 日历订阅 (ICS) 的日历：

* 你可以通过用户界面，而不是通过 Microsoft Graph API 为用户邮箱添加基于 ICS 的日历。
* [列出用户的日历](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_calendars)允许你获取用户默认日历组中或指定日历组中的每个 [日历](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/calendar)的**名称**、**颜色**和 **id** 属性，包括所有基于 ICS 的日历。你无法存储或访问日历资源中的 ICS URL。
* 还可以[列出基于 ICS 的日历事件](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/calendar_list_events)。

### <a name="using-delta-query"></a>使用 delta 查询

有关使用 delta 查询的已知问题，请参阅本文中的 [delta 查询部分](#delta-query)。

## <a name="groups-and-microsoft-teams"></a>组和 Microsoft Teams

>**注意** Microsoft Teams 现在处于预览状态，仅在 Microsoft Graph beta 终结点中可用。

### <a name="policy"></a>策略

使用 Microsoft Graph 创建并命名 Office 365 组会忽略通过 Outlook Web App 配置的所有 Office 365 组策略。 

### <a name="permissions-for-groups-and-microsoft-teams"></a>组和 Microsoft Teams 的权限

Microsoft Graph 公开了两个权限（*Group.Read.All* 和 *Group.ReadWrite.All*）用于访问组和 Microsoft Teams 的 API。这些权限必须征得管理员同意（与预览不同的地方）。我们计划在将来新增可征得用户同意的组和团队的权限。

此外，只有与核心组管理和管理相关的 API 才支持使用委派权限或仅限应用权限进行访问。其他所有的组 API 功能仅支持委派权限。

同时支持委派权限和仅限应用权限的组功能示例：

* 创建和删除组
* 获取和更新与组管理或管理相关的组属性
* 组[目录设置](../api-reference/v1.0/resources/directoryobject.md)、类型和同步
* 组所有者和成员


仅支持委派权限的组功能示例：

* 组对话、事件和照片
* 外部发件人、被接受或拒绝的发件人、组订阅
* 用户收藏夹和未读计数

### <a name="teams-in-microsoft-teams-preview"></a>Microsoft Teams 中的团队（预览）

Microsoft Teams 基于 Office 365 组建立。在“创建组”当前不允许创建团队的异常下，所有组 API 也可以与团队配合使用。将来的 API 版本将支持此功能。

### <a name="microsoft-teams-channels-preview"></a>Microsoft Teams 频道（预览）

目前，你可以读取和创建频道，但无法更新或删除频道。将来的 API 版本将支持此功能。

### <a name="microsoft-teams-chat-threads-and-chat-messages-preview"></a>Microsoft Teams 聊天线程和聊天消息（预览）

目前，你可以在通道中创建聊天线程，但无法读取现有的聊天线程或添加对它们的答复。作为 weel，你无法读取或写入与团队或频道范围外的用户之间的直接聊天。将来的 API 版本将增加此区域中的其他功能。


### <a name="adding-and-getting-attachments-of-group-posts"></a>添加和获取组帖子的附件

向组帖子 [添加](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/post_post_attachments) 附件、[列出](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/post_list_attachments) 和获取组帖子的附件目前返回错误消息“OData 请求不受支持”。已经为 `/v1.0` 和 `/beta` 版本推出修复程序，并预计到 2016 年 1 月底会广泛推出。

### <a name="setting-the-allowexternalsenders-property"></a>设置 allowExternalSenders 属性

目前，`/v1.0` 和 `/beta` 中均存在一个问题，即会阻止在 POST 或 PATCH 操作中设置组的属性 **allowExternalSenders**。

### <a name="using-delta-query"></a>使用 delta 查询

有关使用 delta 查询的已知问题，请参阅本文中的 [delta 查询部分](#delta-query)。

## <a name="contacts"></a>联系人

### <a name="organization-contacts-available-in-only-beta"></a>仅 beta 版支持组织联系人。

目前只支持个人联系人。`/v1.0` 中目前暂不支持组织联系人，但可以在 `/beta` 中找到组织联系人。

### <a name="default-contacts-folder"></a>默认联系人文件夹

在 `/v1.0` 版本中，`GET /me/contactFolders` 不包括用户的默认联系人文件夹。 

将会提供修复程序。同时，您还可以使用以下[列出联系人](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_contacts)查询和 **parentFolderId** 属性作为一种解决方法，来获取默认联系人文件夹的文件夹 ID：

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

在上面的查询中：

1. `/me/contacts?$top=1` 获取默认联系人文件夹中 [联系人](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/contact) 的属性。
2. 附加 `&$select=parentFolderId` 仅返回联系人的 **parentFolderId** 属性，即默认联系人文件夹的 ID。


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a>在 beta 版中通过联系人文件夹访问联系人

目前，`/beta` 版中存在一个问题，即会在 REST 请求 URL 中指定父文件夹，进而阻止访问[联系人](../api-reference/beta/resources/contact.md)，如以下 2 个方案所示。

* 从用户的顶级 [contactFolder](../api-reference/beta/resources/contactfolder.md) 访问联系人。

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* 访问 **contactFolder** 的子文件夹中的联系人。下面的示例展示了一级嵌套，但可以在子文件夹的子级等对象中访问联系人。

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

或者，如下所示，只需指定联系人 ID 即可[获取](../api-reference/beta/api/contact_get.md)此联系人，因为在 `/beta` 版中 GET /contacts 适用于用户邮箱中的所有联系人：

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a>邮件

### <a name="the-comment-parameter-for-creating-a-draft"></a>用于创建草稿的注释参数

用于创建答复或转发草稿的**注释**参数（[createReply](../api-reference/v1.0/api/message_createreply.md)、[createReplyAll](../api-reference/v1.0/api/message_createreplyall.md)、[createForward](../api-reference/v1.0/api/message_createforward.md)）不会成为最终的邮件草稿正文的一部分。  

## <a name="drives-files-and-content-streaming"></a>驱动器、文件和内容流式传输

* 在通过浏览器访问个人站点之前，用户首次通过 Microsoft Graph 访问个人驱动器会生成 401 响应。

## <a name="query-parameter-limitations"></a>查询参数限制

* **$expand** 限制：
    * 不支持 `nextLink`
     * 不支持 1 级以上扩展
     * 不支持其他参数（**$filter**、**$select**）
* 不支持多个命名空间
* 在用户、组、设备、服务主体和应用程序上，不支持对 `$ref` 执行获取操作和投射。
* 不支持 `@odata.bind`。也就是说，开发者无法正确地在组上设置 `Accepted` 或 `RejectedSenders`。
* 使用极少的元数据时，非包容导航（如邮件）上不存在 `@odata.id`
* 跨工作负载筛选/搜索不可用。 
* 全文搜索（使用 **$search**）仅对某些实体（如邮件）可用。

## <a name="delta-query"></a>Delta 查询

* 跟踪关系更改时，OData 上下文有时无法正确返回。
* 架构扩展（旧版）未使用 $select 语句返回，而是在无 $select 的情况下返回。
* 客户端无法跟踪开放扩展或已注册的架构扩展的更改。

## <a name="extensions"></a>扩展

### <a name="change-tracking-is-not-supported"></a>不支持更改跟踪

开放扩展或架构扩展属性不支持更改跟踪（Delta 查询）。

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a>同时创建资源和开放扩展

无法在创建**管理单元**、**设备**、**组**、**组织**或**用户**的实例的同时指定开放扩展。必须首先创建实例，然后在该实例的后续 ``POST`` 请求中指定开放扩展数据。

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a>每个资源实例允许 100 个架构扩展属性值的限制

目录资源（如**设备**、**组**和**用户**）目前将可在资源实例上设置的架构扩展属性值的总数限制为 100。

## <a name="json-batching"></a>JSON 批处理

### <a name="no-nested-batch"></a>无嵌套批处理

JSON 批处理请求中不得包含任何嵌套批处理请求。

### <a name="all-individual-requests-must-be-synchronous"></a>所有单个请求必须同步

批处理请求中包含的所有请求都必须同步执行。如果存在，将忽略 `respond-async` 首选项。

### <a name="no-transactions"></a>无事务

Microsoft Graph 当前不支持单个请求的事务处理。将忽略单个请求的 `atomicityGroup` 属性。

### <a name="uris-must-be-relative"></a>URI 必须相对

始终在批处理请求中指定相对的 URI。Microsoft Graph 将使用批处理 URL 中包含的版本终结点使这些 URL 绝对。

### <a name="limit-on-batch-size"></a>限制批处理大小

JSON 批处理请求目前被限定为 5 个单独请求。当 JSON 批处理成熟时，将引发此限制。

### <a name="simplified-dependencies"></a>简化的依赖项

单独请求可以依赖其他单独请求。目前，请求只能依赖于单个其他请求，并且必须遵循下面的三种模式之一：

1. 平行 - 没有单独的请求在 `dependsOn` 属性中声明依赖项。
2. 串行 - 所有单独请求都依赖于之前的单独请求。
3. 相同 - 在 `dependsOn` 属性中声明依赖项的所有单独请求均声明了相同的依赖项。

当 JSON 批处理成熟时，将删除这些限制。

## <a name="cloud-solution-provider-apps-must-use-azure-ad-endpoint"></a>云解决方案提供商应用必须使用 Azure AD 终结点

云解决方案提供商 (CSP) 应用必须从 Azure AD (v1) 终结点中获取令牌，才能在其合作伙伴托管的客户中成功调用 Microsoft Graph。目前，不支持通过较新的 Azure AD v2.0 终结点获取令牌。

## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a>只有 Office 365 REST 或 Azure AD Graph API 才具有的功能

某些功能尚未在 Microsoft Graph 中提供。如果找不到所需的功能，请使用特定于终结点的 [Office 365 REST API](https://msdn.microsoft.com/en-us/office/office365/api/api-catalog)。有关 Azure Active Directory，请参考 [Microsoft Graph 或 Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) 博客文章，获取只能通过 Azure AD Graph API 提供的功能。

### <a name="feedback"></a>反馈

> 我们非常重视你的反馈意见。请在 [Stack Overflow](http://stackoverflow.com/questions/tagged/microsoftgraph) 上与我们联系。
