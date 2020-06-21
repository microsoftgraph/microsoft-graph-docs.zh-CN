---
title: Microsoft Graph 已知问题
description: 本文介绍了 Microsoft Graph 的已知问题。
author: MSGraphDocsVTeam
localization_priority: Priority
ms.openlocfilehash: 98c61991ec99b1f7776c03f5fa5bc2400b5950a6
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744054"
---
# <a name="known-issues-with-microsoft-graph"></a>Microsoft Graph 已知问题

本文介绍了 Microsoft Graph 的已知问题。 

若要报告已知问题，请参阅[Microsoft Graph 支持](https://developer.microsoft.com/graph/support)页面。

有关 Microsoft Graph API 的最新更新的信息，请参阅[Microsoft graph 更改日志](changelog.md)。

## <a name="bookings"></a>Bookings

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a>查询 bookingBusinesses 时出现 ErrorExceededFindCountLimit

当组织拥有多个预订业务且提出请求的帐户不是管理员时，获取 `bookingBusinesses` 列表会失败，并显示以下错误代码：

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

解决方法是，可以通过加入 `query` 参数来限制请求返回的业务集，例如：

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```
## <a name="calendars"></a>日历

### <a name="accessing-a-shared-calendar"></a>访问共享日历

使用以下操作尝试访问其他用户共享的日历中的事件时：

```http
GET /users/{id}/calendars/{id}/events
```

You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:

- 过去，日历共享的实现方法有两种。为了加以区分，将它们称为“旧”方法和“新”方法。
- 新方法当前可用于通过查看或编辑权限共享日历，但无法通过委派权限进行共享。
- 只有使用**新**方法共享日历后，才能使用日历 REST API 查看或编辑共享日历。
- 如果使用**旧**方法共享日历，则无法使用日历 REST API 查看或编辑此类日历（或其事件）。


如果日历是通过查看或编辑权限共享，但使用的是旧方法，现在可以修复错误，手动将日历共享升级为使用新方法。
随着时间的推移，Outlook 将把所有共享日历（包括通过委托权限共享的日历）自动升级为使用新方法。

若要手动将共享日历升级为使用新方法，请按照以下步骤操作：
1.  收件人删除以前与他们共享的日历。
2.  日历所有者在 Outlook 网页版、iOS 版或 Android 版中重新共享日历。
3.  The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)
4.  收件人可以在 Outlook iOS 版或 Android 版中查看共享日历，从而验证是否已成功使用新方法重新共享日历。

A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:

```http
GET /me/calendars/{id}/events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a>在用户邮箱中添加和访问基于 ICS 的日历

目前，还有部分支持基于 Internet 日历订阅 (ICS) 的日历：

* 你可以通过用户界面，而不是通过 Microsoft Graph API 为用户邮箱添加基于 ICS 的日历。
* [Listing the user's calendars](/graph/api/user-list-calendars?view=graph-rest-1.0) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.
* 还可以[列出基于 ICS 的日历事件](/graph/api/calendar-list-events?view=graph-rest-1.0)。

### <a name="attaching-large-files-to-events"></a>将大型文件附加到事件
尝试[将大型文件附加](outlook-large-attachments.md)到共享或委派的邮箱中的 Outlook 邮件或事件时，具有委派权限的应用将返回 `HTTP 403 Forbidden`。 使用委派权限，仅当邮件或事件在已登录用户的邮箱中时，[createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) 才会成功。

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a>Microsoft Teams 的 onlineMeetingUrl 属性支持

目前，Skype 会议[事件](/graph/api/resources/event?view=graph-rest-1.0)的 **onlineMeetingUrl** 属性指明联机会议 URL。 不过，对于 Microsoft Teams 会议事件，此属性设置为 NULL。

Beta 版本提供了一种变通方法，可以使用 [事件](/graph/api/resources/event?view=graph-rest-beta) 的 **onlineMeetingProvider** 属性来验证提供程序是否为 Microsoft Teams。 通过**事件**的 **** 属性，可以访问 **joinUrl**。

## <a name="change-notifications"></a>更改通知

### <a name="additional-notifications-for-users"></a>其他用户通知

对于“**changeType**”设置为“**updated**” 的“**user**”，[订阅](/graph/api/resources/subscription)以上更改还将收到“**changeType**”的通知：在创建和软删除用户时**已更新**。

### <a name="additional-notifications-for-groups"></a>其他组通知

对于“**changeType**”设置为“**updated**” 的“**group**”，[订阅](/graph/api/resources/subscription)以上更改还将收到“**changeType**”通知：在创建和软删除组时**已更新**。

## <a name="cloud-communications"></a>云通信 

对于通过云通信 API 创建的频道会议，Microsoft Teams 客户端不会显示“**查看会议详细信息**”菜单。

## <a name="cloud-solution-provider-apps"></a>云解决方案提供商应用

### <a name="csp-apps-must-use-azure-ad-endpoint"></a>CSP 应用必须使用 Azure AD 终结点

Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a>对 CSP 应用的预授权不适用于一些客户租户

在某些情况下，对 CSP 应用的预授权可能不适用于一些客户租户。

- 对于使用委派权限的应用，首次将此应用用于新客户租户时，登录后可能会看到以下错误：`AADSTS50000: There was an error issuing a token`。
- 对于使用应用权限的应用，应用可以获取令牌，但在调用 Microsoft Graph 时会意外看到“拒绝访问”消息。

我们正在努力工作，以尽快解决此问题，让预授权适用于所有客户租户。

同时，若要取消阻止开发和测试，可使用以下解决方法。

>**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.

1. Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. 创建 Microsoft Graph 服务主体。

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```
## <a name="contacts"></a>联系人

### <a name="organization-contacts-available-in-only-beta"></a>仅 beta 版支持组织联系人。

Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.

### <a name="default-contacts-folder"></a>默认联系人文件夹

在 `/v1.0` 版本中，`GET /me/contactFolders` 不包括用户的默认联系人文件夹。

A fix will be made available. Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

在上面的查询中：

1. `/me/contacts?$top=1` 获取默认联系人文件夹中 [联系人](/graph/api/resources/contact?view=graph-rest-1.0) 的属性。
2. 附加 `&$select=parentFolderId` 仅返回联系人的 **parentFolderId** 属性，即默认联系人文件夹的 ID。


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a>在 beta 版中通过联系人文件夹访问联系人

目前，`/beta` 版中存在一个问题，即会在 REST 请求 URL 中指定父文件夹，进而阻止访问[联系人](/graph/api/resources/contact?view=graph-rest-beta)，如以下 2 个方案所示。

* 从用户的顶级 [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) 访问联系人。

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

或者，如下所示，只需指定联系人 ID 即可[获取](/graph/api/contact-get?view=graph-rest-beta)此联系人，因为在 `/beta` 版中 GET /contacts 适用于用户邮箱中的所有联系人：

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
## <a name="delta-query"></a>Delta 查询

* 跟踪关系更改时，OData 上下文有时无法正确返回。
* 架构扩展（旧版）未使用 $select 语句返回，而是在无 $select 的情况下返回。
* 客户端无法跟踪开放扩展或已注册的架构扩展的更改。

## <a name="extensions"></a>扩展

### <a name="change-tracking-is-not-supported"></a>不支持更改跟踪

开放扩展或架构扩展属性不支持更改跟踪（Delta 查询）。

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a>同时创建资源和开放扩展

You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a>创建资源实例的同时添加架构扩展数据

不能在创建 **contact**、**event**、**message** 或 **post** 实例的同一个操作中指定架构扩展。
必须先创建资源实例，然后再对此实例执行 `PATCH`，从而添加架构扩展和自定义数据。

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a>每资源实例最多可以添加 100 个架构扩展属性值

目录资源（如**设备**、**组**和**用户**）目前将可在资源实例上设置的架构扩展属性值的总数限制为 100。

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a>并非所有实体类型都支持对架构扩展属性进行筛选

Outlook 实体类型不支持对架构扩展属性进行筛选（使用 `$filter` 表达式）- **联系人**、**事件**、**消息**或**帖子**。

## <a name="files-onedrive"></a>文件 (OneDrive)

* 在通过浏览器访问个人站点之前，用户首次通过 Microsoft Graph 访问个人驱动器会生成 401 响应。

## <a name="groups"></a>组

### <a name="permissions-for-groups-and-microsoft-teams"></a>组和 Microsoft Teams 的权限

Microsoft Graph 为组和 Microsoft Teams 公开了两个用于访问 API 的权限（[*Group.Read.All*](permissions-reference.md#group-permissions) 和 [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)）。
管理员必须同意授予这些权限。
今后，我们计划新增用户可同意授予的组和团队权限。

Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.

同时支持委派权限和仅限应用权限的组功能示例：

* 创建和删除组
* 获取和更新与组管理或管理相关的组属性
* 组[目录设置](/graph/api/resources/directoryobject?view=graph-rest-1.0)、类型和同步
* 组所有者和成员
* 获取组对话和线索

仅支持委派权限的组功能示例：

* 组事件、照片
* 外部发件人、被接受或拒绝的发件人、组订阅
* 用户收藏夹和未看计数

### <a name="policy"></a>策略

使用 Microsoft Graph 创建并命名 Office 365 组会忽略通过 Outlook Web App 配置的所有 Office 365 组策略。

### <a name="setting-the-allowexternalsenders-property"></a>设置 allowExternalSenders 属性

目前，`/v1.0` 和 `/beta` 中均存在一个问题，即会阻止在 POST 或 PATCH 操作中设置组的属性 **allowExternalSenders**。

### <a name="using-delta-query"></a>使用 delta 查询

有关使用 delta 查询的已知问题，请参阅本文中的 [delta 查询部分](#delta-query)。

## <a name="identity-and-access--application-and-service-principal-apis"></a>身份和访问 | 应用程序和服务主体 API

There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) entities currently in development. The following is a summary of current limitations and in-development API features.

当前限制：

* 只有在所有更改完成后，一些应用属性（如 appRoles 和 addIns）才可用。
* 只能注册多租户应用。
* 更新应用仅限于在首次 beta更新后注册的应用。
* Azure Active Directory 用户可以注册应用并添加其他所有者。
* 支持 OpenID Connect 和 OAuth 协议。
* 无法向应用分配策略。
* 无法对需要 appId 的 ownedObjects 执行操作（例如，users/{id|userPrincipalName}/ownedObjects/{id}/...）

处于开发阶段的功能：

* 可以注册单租户应用。
* 更新 servicePrincipal。
* 将现有 Azure AD 应用迁移到更新后的模型中。
* 支持 appRoles、预授权客户端、可选声明、组成员身份声明和品牌塑造
* Microsoft 帐户 (MSA) 用户可以注册应用。
* 支持 SAML 和 WsFed 协议。

## <a name="identity-and-access--conditional-access"></a>身份和访问 | 条件访问

### <a name="permissions"></a>权限

目前调用 POST 和 PATCH API 需要 Policy.Read.All 权限。 将来可以通过 Policy.ReadWrite.ConditionalAccess 权限读取目录中的策略。

## <a name="json-batching"></a>JSON 批处理

### <a name="no-nested-batch"></a>无嵌套批处理

JSON 批处理请求中不得包含任何嵌套批处理请求。

### <a name="all-individual-requests-must-be-synchronous"></a>所有单个请求必须同步

All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.

### <a name="no-transactions"></a>无事务

Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.

### <a name="uris-must-be-relative"></a>URI 必须相对

Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.

### <a name="limit-on-batch-size"></a>限制批处理大小

JSON 批处理请求目前限定为 20 个单独请求。

### <a name="simplified-dependencies"></a>简化的依赖项

Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:

1. 平行 - 没有单独的请求在 `dependsOn` 属性中声明依赖项。
2. 串行 - 所有单独请求都依赖于之前的单独请求。
3. 相同 - 在 `dependsOn` 属性中声明依赖项的所有单独请求均声明了相同的依赖项。

随着 JSON 批处理技术日臻成熟，这些限制将会被取消。

## <a name="mail-outlook"></a>邮件 (Outlook)

### <a name="attaching-large-files-to-messages"></a>将大型文件附加到邮件
尝试[将大型文件附加](outlook-large-attachments.md)到共享或委派的邮箱中的 Outlook 邮件或事件时，具有委派权限的应用将返回 `HTTP 403 Forbidden`。 使用委派权限，仅当邮件或事件在已登录用户的邮箱中时，[createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) 才会成功。

### <a name="the-comment-parameter-for-creating-a-draft"></a>用于创建草稿的注释参数

用于创建答复或转发草稿的**注释**参数（[createReply](/graph/api/message-createreply?view=graph-rest-1.0)、[createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0)、[createForward](/graph/api/message-createforward?view=graph-rest-1.0)）不会成为最终的邮件草稿正文的一部分。

### <a name="get-messages-returns-chats-in-microsoft-teams"></a>GET 消息返回 Microsoft Teams 中的聊天

在 v1 和 beta 终结点中，`GET /users/id/messages` 的响应包含出现在团队或通道范围外的用户的 Microsoft Teams 聊天。 这些聊天消息具有“即时信息”作为其主题。

## <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

### <a name="get-teams-is-not-supported"></a>不支持 GET /teams

若要获取团队列表，请参阅[列出所有团队](teams-list-all-teams.md)和[列出你的团队](/graph/api/user-list-joinedteams?view=graph-rest-1.0)。

### <a name="post-teams-is-only-available-in-beta"></a>POST /teams 仅适用于 beta 版
若要在 v1.0 中创建团队，请参阅[创建团队](/graph/api/team-put-teams?view=graph-rest-1.0)。

### <a name="missing-teams-in-list-all-teams"></a>“列出所有团队”没有列出的团队

[列出所有团队](teams-list-all-teams.md)没有列出过去创建但 Microsoft Teams 用户最近未使用的一些团队。
新团队会被列出。
一些旧团队没有包含“Team”的 **resourceProvisioningOptions** 属性，但新创建的团队和在 Microsoft Teams 中被访问的团队有此属性。
今后，我们将对尚未在 Microsoft Teams 中打开的现有团队设置 **resourceProvisioningOptions**。

## <a name="users"></a>用户

### <a name="no-instant-access-after-creation"></a>创建后无法即时访问

Users can be created immediately through a POST on the user entity. An Office 365 license must first be assigned to a user, in order to get access to Office 365 services. Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API. During this time, apps will receive a 404 HTTP error response.

### <a name="photo-restrictions"></a>照片限制

Reading and updating a user's profile photo is only possible if the user has a mailbox. Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource.
Failure to read or update a photo, in this case, would result in the following error:

```javascript
{
  "error": {
    "code": "ErrorNonExistentMailbox",
    "message": "The SMTP address has no mailbox associated with it."
  }
}
```

### <a name="using-delta-query"></a>使用 delta 查询

有关使用 delta 查询的已知问题，请参阅本文中的 [delta 查询部分](#delta-query)。

### <a name="revoke-sign-in-sessions-returns-wrong-http-code"></a>调用登录会话返回了错误的 HTTP 代码

[用户: revokeSignInSessions API](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) 返回 `204 No content` 响应表示成功调用；如果请求出现任何错误，则返回 HTTP 错误代码（4xx 或 5xx）。  但是，由于服务问题，此 API 会返回 `200 OK` 和始终为 true 的布尔值参数。  在此问题得到修复之前，简单建议开发人员将所有 2xx 返回代码看作此 API 成功。

### <a name="incomplete-objects-when-using-getbyids-request"></a>使用 getByIds 请求时对象完整

使用[获取 ID 列表中的目录对象](/graph/api/directoryobject-getbyids?view=graph-rest-1.0)请求对象应返回完整对象。 但是，当前返回的 v1.0 端点上的[用户](/graph/api/resources/user?view=graph-rest-1.0)对象具有一组有限的属性。 作为临时解决方法，当您将该操作与 `$select` 查询选项结合使用时, 将返回更完整的[用户](/graph/api/resources/user?view=graph-rest-1.0)对象。 此行为不符合 OData 规范。 由于此行为可能在将来更新，因此仅在你提供 `$select=` 以及感兴趣的所有属性时，并且仅当此解决方法的未来重大更改可接受时，才使用此解决方法。

## <a name="query-parameter-limitations"></a>查询参数限制

* 不支持多个命名空间。
* 在用户、组、设备、服务主体和应用程序上，不支持对 `$ref` 执行 GET 操作和投影。
* `@odata.bind` is not supported.  This means that developers won’t be able to properly set the **acceptedSenders** or **rejectedSenders** navigation property on a group.
* 使用极少的元数据时，非包容导航（如邮件）上不存在 `@odata.id`。
* `$expand`:
  * 不支持 `nextLink`
  * 不支持 1 级以上扩展
  * 不支持其他参数（`$filter`、`$select`）
* `$filter`:
  * `/attachments` 终结点不支持筛选器。 如果存在，将忽略 `$filter` 参数。
  * 不支持跨工作负载筛选。
* `$search`:
  * 全文搜索仅对实体子集（如邮件）可用。
  * 不支持跨工作负载搜索。


## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a>只有 Office 365 REST 或 Azure AD Graph API 才具有的功能

某些功能尚未在 Microsoft Graph 中提供。 如果找不到所需的功能，请使用特定于终结点的 [Office 365 REST API](https://docs.microsoft.com/previous-versions/office/office-365-api/)。 有关 Azure Active Directory 的信息，请参阅[将 Azure AD Graph 应用迁移到 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)。 
