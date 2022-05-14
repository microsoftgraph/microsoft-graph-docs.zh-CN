---
title: 使用增量查询跟踪 Microsoft Graph 数据更改
description: Delta 查询使应用程序能够发现新创建、更新或删除的实体，无需使用每个请求对目标资源执行完全读取。Microsoft Graph 应用程序可以使用 delta 查询和本地数据存储高效地同步更改。
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 714fac5350f7df2222ca563b9660994431a3b382
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398571"
---
# <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a>使用 delta 查询跟踪 Microsoft Graph 数据变更

Delta 查询使应用程序能够发现新创建、更新或删除的实体，无需使用每个请求对目标资源执行完全读取。Microsoft Graph 应用程序可以使用 delta 查询和本地数据存储高效地同步更改。

> [!div class="nextstepaction"]
> [教程：在 Microsoft Graph 上使用“更改通知”和“跟踪更改”](/learn/modules/msgraph-changenotifications-trackchanges)

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>使用 delta 查询来跟踪资源集合的更改

通常的调用模式如下：

1. 应用程序首先对所需资源运行 delta 函数以调用 GET 请求。
2. Microsoft Graph 发送一个包含已请求资源和[状态令牌](#state-tokens)的响应。

     a.如果返回了 `@odata.nextLink` URL，则会话中可能存在要检索的其他数据页面。应用程序继续使用 `@odata.nextLink` URL 发出请求以检索所有页面中的数据，直到响应中返回 `@odata.deltaLink` URL。

     b.如果返回了 `@odata.deltaLink` URL，则未返回关于资源现有状态的更多数据。为了执行以后的请求，应用程序使用 `@odata.deltaLink` URL 了解资源更改。

3. 当应用程序需要了解资源更改时，会使用步骤 2 中收到的 `@odata.deltaLink` URL 发出新请求。*可能* 在完成步骤 2 或应用程序检查更改时立即发出此请求。
4. Microsoft Graph 返回响应（`@odata.nextLink` URL 或 `@odata.deltaLink` URL），其中描述了自上一个请求以来的资源变更。

>**注意：** Azure Active Directory 中存储的资源（如用户和组）支持“从现在开始同步”方案。 这样一来，便可以跳过第 1 步和第 2 步（如果不想检索资源完整状态的话），并改为请求获取最新 `@odata.deltaLink`。 将 `$deltaToken=latest` 追加到 `delta` 函数中，这样响应就会包含 `@odata.deltaLink`，而不包含资源数据。 OneDrive 和 SharePoint 中的资源也支持此功能。 有关 OneDrive 和 SharePoint 中的资源，请改为附加 `token=latest` 。

>**注意：** 引用增量查询函数的方式通常是将 `/delta` 附加到资源名称。 但是，`/delta` 是在 Microsoft Graph SDK 生成的请求中显示的完全限定名称 `/microsoft.graph.delta` 的快捷方式。

>**注意：** 对增量查询函数的初始请求（没有 `$deltaToken` 或 `$skipToken`）将返回集合中当前存在的资源。 初始 delta 查询之前创建并已删除的资源不会返回。 初始请求前进行的更新在返回的资源上按其最新状态进行汇总。

### <a name="state-tokens"></a>状态令牌

增量查询 GET 响应中始终返回 `@odata.nextLink` 或 `@odata.deltaLink` 响应头中指定的 URL。`@odata.nextLink` URL 包含的是 `$skipToken`，`@odata.deltaLink` URL 包含的是 `$deltaToken`。

这些令牌对客户端不透明。以下是需要了解的详细信息：

- 每个令牌都反映状态，并表示一轮更改跟踪中的响应快照。

- 状态令牌还会进行编码，并包括初始 delta 查询请求中指定的其他查询参数（如 `$select`）。因此，不需要在后续 delta 查询请求中重复这些操作。

- 执行增量查询时，可以将 `@odata.nextLink` 或 `@odata.deltaLink` URL 复制并应用到下一个 **delta** 函数调用，无需检查 URL 的内容（包括其状态令牌）。

### <a name="optional-query-parameters"></a>可选的查询参数

如果客户使用查询参数，则它必须在初始请求中指定。Microsoft Graph 自动将指定参数编码为响应中提供的 `@odata.nextLink` 或 `@odata.deltaLink`。调用应用程序只需预先指定查询参数一次。Microsoft Graph 将为所有后续请求自动添加指定参数。

请注意以下可选查询参数的常规有限支持：

- `$orderby`

    不要假定从增量查询返回的响应的特定序列。假定同一项可以显示在 `@odata.nextLink` 序列中的任何位置，并在合并逻辑中处理它。
- `$top`

    每页中的对象数量可能因资源类型和资源更改类型而异。

对于[消息](/graph/api/resources/message)资源，请参阅[增量查询中的查询参数支持](delta-query-messages.md#use-query-parameters-in-a-delta-query-for-messages)的详细信息。

对于[用户](/graph/api/resources/user)和[组](/graph/api/resources/group)资源，在使用某些查询参数时受到限制：

- 不支持 `$expand`。
- 不支持 `$top`。
- 不支持 `$orderby`。
- 如果使用的是 `$select` 查询参数，则该参数表示客户倾向于仅跟踪 `$select` 语句中指定的属性或关系的更改。如果未选中的属性发生更改，则属性已更改的资源将不会出现在后续请求之后的 delta 响应中。
- `$select` 还分别支持用户和组的 **管理** 器和 **成员** 导航属性。 选择这些属性可以跟踪对用户管理器和组成员身份的更改。

- 使用范围筛选器可以按对象 ID 跟踪对一个或多个特定用户或组所做的更改。例如，以下请求返回与查询筛选器中指定的 ID 匹配的组所做的更改。

<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
https://graph.microsoft.com/beta/groups/delta/?$filter=id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ae5f' or id eq '004d6a07-fe70-4b92-add5-e6e37b8acd8e'
```

## <a name="resource-representation-in-the-delta-query-response"></a>delta 查询响应中的资源表示形式

- 在 delta 查询响应中，使用标准表示形式表示受支持资源的新建实例。

- 更新实例由它们的 **id** 表示，*至少* 具有已更新的属性，但可能也包含其他属性。

- 用户和组上的关系表示为标准资源表示形式的注释。这些批注使用格式 **propertyName@delta**。批注包含在初始增量查询请求的响应中。

删除的实例由它们的 **id** 和 **@removed** 对象表示。 **@removed** 对象可能包含有关删除实例的原因的附加信息。 例如，`"@removed": {"reason": "changed"}`。

可能的 **@removed** 原因可以是`changed` 或 `deleted`。

- `changed`表示该项已被删除，可以从 [deletedItems](/graph/api/resources/directory) 恢复。

- `deleted`表示该项已被删除，无法恢复。

在初始的 delta 查询响应和跟踪的 (deltaLink) 响应中，可以返回 **@removed** 对象。使用 delta 查询请求的客户端应应被设计为处理响应中的这些对象。

>**注意：** 在响应中可能会多次包含一个实体，前提是多次在特定情况下更改了该实体。 增量查询可以使应用程序列出所有更改，但不能确保实体在单个响应中是统一的。

## <a name="supported-resources"></a>支持的资源

以下资源当前支持 Delta 查询。请注意，v1.0 中提供的某些资源相应的 **delta** 函数仍处于预览状态，如所示。

| **资源集合**                                        | **API**                                                                                                                                                      |
| :------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 应用程序                                                   | [application](/graph/api/resources/application) 资源的 [delta](/graph/api/application-delta) 函数                                               |
| 管理单元（预览版）                                 | [administrativeUnit](/graph/api/resources/administrativeunit) 资源的 [delta](/graph/api/administrativeunit-delta) 函数（预览版）                |
| 作业类别                                          | [educationCategory](/graph/api/resources/educationcategory) 资源的 [delta](/graph/api/educationcategory-delta) 函数                                    |
| 频道中的聊天消息                                     | [chatMessage](/graph/api/resources/chatmessage) 的 [delta](/graph/api/chatmessage-delta) 函数（预览版）                                              |
| 目录角色                                                | [directoryRole](/graph/api/resources/directoryrole) 资源的 [delta](/graph/api/directoryrole-delta) 函数 |
| 驱动器项目\*                                                  | [driveItem](/graph/api/resources/driveitem) 资源的 [delta](/graph/api/driveitem-delta) 函数             |
| 教育作业                                          | [educationAssignment](/graph/api/resources/educationassignment) 资源的 [delta](/graph/api/educationassignment-delta) 函数                                    |
| 教育课堂                                              | [educationClass](/graph/api/resources/educationclass) 资源的 [delta](/graph/api/educationclass-delta) 函数                                      |
| 教育用户                                                | [educationUser](/graph/api/resources/educationuser) 资源的 [delta](/graph/api/educationuser-delta) 函数                                         |
| 教育学校                                              | [educationSchool](/graph/api/resources/educationschool) 资源的 [delta](/graph/api/educationschool-delta) 函数                                   |
| 主日历的日历视图（日期范围）中的事件 | [事件](/graph/api/resources/event)资源的 [delta](/graph/api/event-delta) 函数                         |
| 组                                                         | [组](/graph/api/resources/group)资源的 [delta](/graph/api/group-delta) 函数                         |
| 邮件文件夹                                                   | [邮件文件夹](/graph/api/resources/mailfolder)资源的 [delta](/graph/api/mailfolder-delta) 函数          |
| 文件夹中的邮件                                           | [邮件](/graph/api/resources/message)资源的 [delta](/graph/api/message-delta) 函数                   |
| 组织联系人                                        | [orgContact](/graph/api/resources/orgcontact) 资源的 [delta](/graph/api/orgcontact-delta) 函数          |
| OAuth2PermissionGrants                                         | [oauth2permissiongrant](/graph/api/resources/oauth2permissiongrant) 资源的 [delta](/graph/api/oauth2permissiongrant-delta) 函数                 |
| 私人联系人文件夹                                       | [联系人文件夹](/graph/api/resources/contactfolder)资源的 [delta](/graph/api/contactfolder-delta) 函数 |
| 文件夹中的私人联系人                                  | [contact](/graph/api/resources/contact) 资源的 [delta](/graph/api/contact-delta) 函数                   |
| Planner 项目\*\*（预览版）                                    | [plannerUser](/graph/api/resources/planneruser) 资源所有段的 [delta](/graph/api/planneruser-list-delta) 函数（预览版）                 |
| 服务主体                                             | [servicePrincipal](/graph/api/resources/serviceprincipal) 资源的 [delta](/graph/api/serviceprincipal-delta) 函数                                |
| 任务列表中的任务                                           | [todoTask](/graph/api/resources/todotask) 资源的 [delta](/graph/api/todotask-delta) 函数                                                        |
| 任务列表                                                     | [todoTaskList](/graph/api/resources/todotasklist) 资源的 [delta](/graph/api/todotasklist-delta) 函数                                            |
| 用户                                                          | [用户](/graph/api/resources/user)资源的 [delta](/graph/api/user-delta) 函数                            |


> \* OneDrive 资源的使用模式与其他支持资源类似，仅存在一些小的语法差异。为了与其他资源类型保持一致，适用于驱动器的 delta 查询今后将进行更新。若要详细了解现行语法，请参阅[跟踪驱动器更改](/graph/api/driveitem-delta)。

> \*\* Planner 资源的使用模式与其他受支持的资源类似，但存在一些差异。 有关详细信息，请参阅[查看 Planner 的更改](/graph/api/planneruser-list-delta)。

## <a name="limitations"></a>限制

### <a name="properties-stored-outside-of-the-main-data-store"></a>在主数据存储外部存储的属性

某些资源包含一些存储在资源主数据存储外部的属性（例如，用户资源大部分存储在 Azure AD 系统中，而 **skills** 之类的一些属性存储在 SharePoint Online 中）。 目前，在更改跟踪中不支持这些属性；对其中一个属性所做的更改不会导致在增量查询响应中显示对象。 目前，仅在主数据存储中存储的属性会触发增量查询中的更改。

若要验证属性是否可用于增量查询，请尝试对资源集合执行常规 `GET` 操作，然后选择感兴趣的属性。例如，可以在用户集合上尝试 **skills** 属性。

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/?$select=skills
```

由于 **skills** 属性存储在 Azure AD 外部，因此响应如下。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 501 Not Implemented
Content-type: application/json

{
    "error": {
        "code": "NotImplemented",
        "message": "This operation target is not yet supported.",
        "innerError": {
            "request-id": "...",
            "date": "2019-09-20T21:47:50"
        }
    }
}
```

据此可得知，**user** 资源的增量查询不支持 **skills** 属性。

### <a name="navigation-properties"></a>导航属性

不支持导航属性。例如，不能跟踪对用户集合所做的更改，这些更改将包含对用户 **photo** 属性所做的更改；**photo** 是一个存储在用户实体之外的导航属性，且对其进行的更改不会导致增量响应中包含用户对象。

### <a name="processing-delays"></a>处理延迟

对资源实例进行更改（可通过应用界面或 API 进行）的时间与所做的更改反映在增量查询响应中的时间之间可能会出现不同的延迟。

有时，当你选择 `@odata.nextLink` 或 `@odata.deltaLink` 时，可能无法指示对于对象所做的更改。 这是因为某些请求可能对最近创建、更新或删除的对象具有复制延迟。 请在一段时间后重试 `@odata.nextLink` 或 `@odata.deltaLink` 以检索最新更改。

### <a name="national-clouds"></a>国家云

增量查询仅适用于公共云和由世纪互联运营的 Microsoft Graph（中国）托管的客户。

### <a name="replays"></a>重新发送

应用程序必须为重播做好准备，重新发送是在后续响应中出现相同更改时发生的。 虽然 delta 查询会尽力减少重新发送，但这种情况还是有可能发生。

### <a name="synchronization-reset"></a>同步重置

Delta 查询可以返回一个`410 (gone)`响应代码和一个 **Location** 标头，其中包含一个空的`$deltaToken`请求 URL（与初始查询相同）。 这表示应用程序必须在目标租户的完全同步的情况下重启。 发生这种情况的原因通常是由于目标租户的内部维护或迁移导致数据不一致。

### <a name="token-duration"></a>令牌持续时间

增量令牌仅在客户端应用程序需要再次运行完整同步前的特定时间段内有效。
+ [目录对象](/graph/api/resources/directoryobject)的时限为 7 天内。 
+ 教育对象（**educationSchool**、**educationUser** 和 **educationClass**）的时限为 7 天内。
+ Outlook 实体（**邮件**、**邮件文件夹**、**事件**、**联系人**、**联系人文件夹**、**待办事项** 和 **待办事项列表**）没有固定时间上限，取决于内部 delta 令牌缓存的大小。 因为缓存中不断添加新 delta 令牌，因此超过缓存容量后，旧 delta 令牌将被删除。

如果令牌过期，服务应响应 40X 系列错误，并显示错误代码，如 `syncStateNotFound`。 有关详细信息，请参阅 [Microsoft Graph](/graph/errors#code-property) 中的错误代码。

## <a name="prerequisites"></a>先决条件

在对某个特定资源执行 delta 查询时也需要读取该资源所需的相同[权限](./permissions-reference.md)。

## <a name="delta-query-request-examples"></a>delta 查询请求示例

- [获取日历视图中事件的增量更改](delta-query-events.md)
- [获取文件夹中邮件的增量更改](./delta-query-messages.md)
- [获取组的增量更改](./delta-query-groups.md)
- [获取用户的增量更改](./delta-query-users.md)
