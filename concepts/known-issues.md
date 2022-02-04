---
title: Microsoft Graph 已知问题
description: 本文介绍了 Microsoft Graph 已知问题。
author: MSGraphDocsVTeam
ms.localizationpriority: high
---

# <a name="known-issues-with-microsoft-graph"></a>Microsoft Graph 已知问题

本文介绍了 Microsoft Graph 已知问题。 

若要报告已知问题，请参阅 [Microsoft Graph 支持](https://developer.microsoft.com/graph/support) 页面。

若要了解 Microsoft Graph API 的最新更新，请参阅 [Microsoft Graph 更改日志](changelog.md)。

## <a name="applications"></a>应用程序

### <a name="some-limitations-apply-to-the-application-and-serviceprincipal-resources"></a>应用程序和 servicePrincipal 资源存在一些限制

[应用程序](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) 和 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) 资源的更改当前处于开发阶段。下面总结了当前的限制和处于开发阶段的 API 功能。

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

### <a name="azure-ad-v20-endpoint-is-not-supported-for-csp-apps"></a>CSP 应用不支持使用 Azure AD v2.0 终结点

云解决方案提供商 (CSP) 应用必须从 Azure AD (v1) 终结点中获取令牌，才能在其合作伙伴托管的客户中成功调用 Microsoft Graph。目前，不支持通过较新的 Azure AD v2.0 终结点获取令牌。

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a>对 CSP 应用的预授权不适用于一些客户租户

在某些情况下，对云解决方案提供商 (CSP) 应用的预授权可能不适用于一些客户租户。

- 对于使用委派权限的应用，首次将此应用用于新客户租户时，登录后可能会看到以下错误：`AADSTS50000: There was an error issuing a token`。
- 对于使用应用权限的应用，应用可以获取令牌，但在调用 Microsoft Graph 时会意外看到“拒绝访问”消息。

我们正在努力工作，以尽快解决此问题，让预授权适用于所有客户租户。

同时，若要取消阻止开发和测试，可使用以下解决方法。

>**注意：** 这不是永久性解决方案，仅用于取消阻止开发。一旦上述问题得到解决，便无需使用此解决方案。在问题得到解决后，无需撤消此解决方法。

1. 打开 Azure AD v2 PowerShell 会话，然后在登录窗口中输入管理员凭据，以连接 `customer` 租户。可以单击[此处](https://www.powershellgallery.com/packages/AzureAD)，下载并安装 Azure AD PowerShell V2。

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. 创建 Microsoft Graph 服务主体。

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```
## <a name="bookings"></a>Bookings

### <a name="error-when-querying-bookingbusinesses"></a>查询 bookingBusinesses 时出错

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

```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```
## <a name="calendar"></a>日历

### <a name="error-accessing-a-shared-calendar"></a>访问共享日历时出错

使用以下操作尝试访问其他用户共享的日历中的事件时：

```http
GET /users/{id}/calendars/{id}/events
```

可能会看到错误代码为 `ErrorInternalServerTransientError` 的 HTTP 500。导致错误发生的原因是：

- 过去，日历共享的实现方法有两种。为了加以区分，将它们称为“旧”方法和“新”方法。
- 新方法当前可用于通过查看或编辑权限共享日历，但无法通过委派权限进行共享。
- 只有使用 **新** 方法共享日历后，才能使用日历 REST API 查看或编辑共享日历。
- 如果使用 **旧** 方法共享日历，则无法使用日历 REST API 查看或编辑此类日历（或其事件）。


如果日历是通过查看或编辑权限共享，但使用的是旧方法，现在可以修复错误，手动将日历共享升级为使用新方法。
随着时间的推移，Outlook 将把所有共享日历（包括通过委托权限共享的日历）自动升级为使用新方法。

若要手动将共享日历升级为使用新方法，请按照以下步骤操作：
1.  收件人删除以前与他们共享的日历。
2.  日历所有者在 Outlook 网页版、iOS 版或 Android 版中重新共享日历。
3.  收件人使用 Outlook 网页版重新接受共享日历。（很快就可以使用其他 Outlook 客户端了。）
4.  收件人可以在 Outlook iOS 版或 Android 版中查看共享日历，从而验证是否已成功使用新方法重新共享日历。

使用新方法共享的日历看起来与邮箱中的其他日历一样。可以使用日历 REST API 查看或编辑共享日历中的事件，就像查看或编辑自己日历中的事件一样。示例：

```http
GET /me/calendars/{id}/events
```

### <a name="partial-support-for-adding-and-accessing-ics-based-calendars-in-users-mailbox"></a>在用户邮箱中添加和访问基于 ICS 的日历的部分支持

目前，仅部分支持基于 Internet 日历订阅 (ICS) 的日历：

* 你可以通过用户界面，而不是通过 Microsoft Graph API 为用户邮箱添加基于 ICS 的日历。
* [列出用户的日历](/graph/api/user-list-calendars)允许你获取用户默认日历组中或指定日历组中的每个 [日历](/graph/api/resources/calendar)的 **名称**、**颜色** 和 **id** 属性，包括所有基于 ICS 的日历。你无法存储或访问日历资源中的 ICS URL。
* 还可以[列出基于 ICS 的日历事件](/graph/api/calendar-list-events)。

### <a name="error-attaching-large-files-to-events"></a>将大文件附加到事件时出错
尝试[将大型文件附加](outlook-large-attachments.md)到共享或委派的邮箱中的 Outlook 邮件或事件时，具有委派权限的应用将返回 `HTTP 403 Forbidden`。 使用委派权限，仅当邮件或事件在已登录用户的邮箱中时，[createUploadSession](/graph/api/attachment-createuploadsession) 才会成功。

### <a name="onlinemeetingurl-property-is-not-supported-for-microsoft-teams"></a>Microsoft Teams 不支持 onlineMeetingUrl 属性

目前，Skype 会议 [事件](/graph/api/resources/event)的 **onlineMeetingUrl** 属性指明联机会议 URL。 不过，对于 Microsoft Teams 会议事件，此属性设置为 NULL。

Beta 版本提供了一种解决方法，可以使用 [事件](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) 的 **onlineMeetingProvider** 属性来验证提供商是否为 Microsoft Teams。 通过 **事件** 的  属性，可以访问 **joinUrl**。

## <a name="change-notifications"></a>更改通知

### <a name="update-notifications-occur-on-creation-and-soft-deletion-of-users"></a>更新通知在创建和软删除用户时发生

对于“**changeType**”设置为“**updated**” 的“**user**”，[订阅](/graph/api/resources/subscription)以上更改还将收到“**changeType**”的通知：在创建和软删除用户时 **已更新**。

### <a name="update-notifications-occur-on-creation-and-soft-deletion-of-groups"></a>更新通知在创建和软删除组时发生

对于“**changeType**”设置为“**updated**” 的“**group**”，[订阅](/graph/api/resources/subscription)以上更改还将收到“**changeType**”通知：在创建和软删除组时 **已更新**。

## <a name="cloud-communications"></a>云通信 

### <a name="view-meeting-details-menu-is-not-available-on-microsoft-teams-client"></a>Microsoft Teams 客户端上不提供“查看会议详细信息”菜单

对于通过云通信 API 创建的频道会议，Microsoft Teams 客户端不会显示“**查看会议详细信息**”菜单。

## <a name="contacts"></a>联系人

### <a name="get-operation-does-not-return-default-contacts-folder"></a>GET 操作不会返回默认联系人文件夹

在 `/v1.0` 版本中，`GET /me/contactFolders` 不包括用户的默认联系人文件夹。

将会提供修复程序。同时，您还可以使用以下 [列出联系人](/graph/api/user-list-contacts)查询和 **parentFolderId** 属性作为一种解决方法，来获取默认联系人文件夹的文件夹 ID：

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

在此请求中：

1. `/me/contacts?$top=1` 获取默认联系人文件夹中 [联系人](/graph/api/resources/contact) 的属性。
2. 附加 `&$select=parentFolderId` 仅返回联系人的 **parentFolderId** 属性，即默认联系人文件夹的 ID。


### <a name="accessing-contacts-via-a-contact-folder-doesnt-work-in-beta"></a>通过联系人文件夹访问联系人在 beta 版中不起作用

目前，`/beta` 版中存在一个问题，即会在 REST 请求 URL 中指定父文件夹，从而阻止访问[联系人](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true)，如以下两种情况所示。

访问用户的顶级 [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta&preserve-view=true) 中的联系人：

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

访问 **contactFolder** 的子文件夹中的联系人： 

```http
GET /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

上面的示例展示了一级嵌套，但也可以访问子文件夹的子文件夹中的联系人，并以此类推。

或者也可以按照示例仅通过指定联系人 ID 来[获取](/graph/api/contact-get?view=graph-rest-beta&preserve-view=true)此联系人，因为 `/beta` 版本中的 GET /contacts 适用于用户邮箱中的所有联系人：

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
## <a name="delta-query"></a>Delta 查询

### <a name="odata-context-is-returned-incorrectly"></a>OData 上下文返回不正确

跟踪关系更改时，OData 上下文有时无法正确返回。

### <a name="schema-extensions-are-not-returned-with-select"></a>架构扩展未使用 `select` 返回

架构扩展（旧版）未使用 `$select` 语句返回，而是在不带有 `$select` 的情况下返回。

### <a name="clients-cannot-track-changes-to-open-extensions"></a>客户端无法跟踪开放扩展的更改。

客户端无法跟踪开放扩展或已注册的架构扩展的更改。

## <a name="devices-and-apps--device-updates-windows-updates"></a>设备和应用|设备更新（Windows 更新）

### <a name="accessing-and-updating-deployment-audiences-is-not-supported"></a>不支持访问和更新部署访问群体。

当前不支持访问和更新通过 Intune 创建的 **部署** 资源上的部署访问群体。

* [列出部署访问群体成员](/graph/api/windowsupdates-deploymentaudience-list-members) 和 [列出部署访问群体排除项](/graph/api/windowsupdates-deploymentaudience-list-exclusions) 返回 `404 Not Found`。
* [更新部署访问群体成员和排除项](/graph/api/windowsupdates-deploymentaudience-updateaudience) 或 [按 ID 更新](/graph/api/windowsupdates-deploymentaudience-updateaudiencebyid) 返回 `202 Accepted`，但不更新访问群体。

## <a name="extensions"></a>扩展

### <a name="change-tracking-is-not-supported"></a>不支持更改跟踪

开放扩展或架构扩展属性不支持更改跟踪（Delta 查询）。

### <a name="unable-to-create-a-resource-and-open-extension-at-the-same-time"></a>无法同时创建资源和开放扩展

无法在创建 **管理单元**、**设备**、**组**、**组织** 或 **用户** 的实例的同时指定开放扩展。必须首先创建实例，然后在该实例的后续 ``POST`` 请求中指定开放扩展数据。

### <a name="unable-to-create-a-resource-instance-and-add-schema-extension-data-at-the-same-time"></a>无法同时创建资源实例和添加架构扩展数据

不能在创建 **contact**、**event**、**message** 或 **post** 实例的同一个操作中指定架构扩展。
必须先创建资源实例，然后再对此实例执行 `PATCH`，从而添加架构扩展和自定义数据。

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a>每资源实例最多可以添加 100 个架构扩展属性值

目录资源（如 **设备**、**组** 和 **用户**）目前将可在资源实例上设置的架构扩展属性值的总数限制为 100。

### <a name="owner-must-be-specified-when-updating-a-schemaextension-definition-using-microsoft-graph-explorer"></a>使用 Microsoft Graph 浏览器更新 schemaExtension 定义时，必须指定所有者

当使用`PATCH` 使用 Graph 浏览器更新 schemaExtension 时，必须指定 **所有者** 属性并将其设置为其当前`appid`值（该值必须是您所拥有的应用程序的 `appId`）。 对于 `appId` 与 **所有者** 不同的任何客户端应用程序，也是如此。

### <a name="filtering-on-schema-extension-properties-is-not-supported-on-all-entity-types"></a>并非所有实体类型都支持对架构扩展属性进行筛选

Outlook 实体类型不支持对架构扩展属性进行筛选（使用 `$filter` 表达式）- **联系人**、**事件**、**消息** 或 **帖子**。

## <a name="files-onedrive"></a>文件 (OneDrive)

### <a name="accessing-a-users-drive-before-user-accesses-it-leads-to-error"></a>在用户访问用户驱动器之前访问它会导致错误

在通过浏览器访问个人网站之前，用户首次通过 Microsoft Graph 访问个人驱动器会生成 `401` 响应。

## <a name="groups"></a>组

### <a name="admins-must-consent-to-permissions-for-groups-and-microsoft-teams"></a>管理员必须同意授予组和 Microsoft Teams 权限

Microsoft Graph 为组和 Microsoft Teams 公开了两个用于访问 API 的权限（[*Group.Read.All*](permissions-reference.md#group-permissions) 和 [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)）。
管理员必须同意授予这些权限。
今后，我们计划新增用户可同意授予的组和 Teams 权限。

### <a name="some-group-apis-dont-support-delegated-or-app-only-permissions"></a>某些组 API 不支持委派权限或仅应用权限

只有与核心组管理相关的 API 才支持使用委派权限或仅限应用权限进行访问。其他所有的组 API 功能仅支持委派权限。

同时支持委派权限和仅限应用权限的组功能示例：

* 创建和删除组
* 获取和更新与组管理或管理相关的组属性
* 组[目录设置](/graph/api/resources/directoryobject)、类型和同步
* 组所有者和成员
* 正在获取组对话和线程

仅支持委派权限的组功能示例：

* 将事件、照片分组
* 外部发件人、被接受或拒绝的发件人、组订阅
* 用户收藏夹和未看计数

### <a name="microsoft-graph-bypasses-group-policies-configured-through-outlook-on-the-web"></a>Microsoft Graph 会绕过通过 Outlook 网页版配置的组策略

使用 Microsoft Graph 创建并命名 Microsoft 365 组时，会忽略通过 Outlook 网页版配置的所有 Microsoft 365 组策略。

### <a name="allowexternalsenders-property-can-only-be-accessed-on-unified-groups"></a>只能在统一组上访问 allowExternalSenders 属性

目前，`/v1.0` 和 `/beta` 中均存在一个问题，即会阻止在 POST 或 PATCH 操作中设置组的属性 **allowExternalSenders**。

只能在统一组上访问 **allowExternalSenders** 属性。 访问安全组上的此属性（包括通过 GET 操作）将导致错误。

### <a name="removing-a-group-owner-also-removes-the-user-as-a-group-member"></a>删除组所有者还将删除作为组成员的用户

在为与 [团队](/graph/api/resources/team.md) 关联的组调用 [DELETE /groups/{id}/owners](/graph/api/group-delete-owners.md) 时，还会从 /groups/{id}/members 列表中删除用户。 要解决此问题，请从所有者和成员中移除用户，然后等待 10 秒，再将其添加回成员。

## <a name="identity-and-access"></a>身份和访问

### <a name="conditional-access-policy-requires-consent-to-permission"></a>条件访问策略需要同意授权

[conditionalAccessPolicy](/graph/api/resources/conditionalaccesspolicy) API 当前需要同意 **Policy.Read.All** 权限才能调用 POST 和 PATCH 方法。 将来可以通过 **Policy.ReadWrite.ConditionalAccess** 权限读取目录中的策略。

### <a name="claims-mapping-policy-might-require-consent-to-permissions"></a>声明映射策略可能需要同意授权

[claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy) API 可能需要得到 `LIST /policies/claimsMappingPolicies` 和 `GET /policies/claimsMappingPolicies/{id}` 方法的 **Policy.Read.All** 和 **Policy.ReadWrite.ConditionalAccess** 授权，如下所示：

+ 如果没有 **claimsMappingPolicy** 对象可用于在 LIST 操作中检索，则任一权限都足以调用此方法。
+ 如果存在要检索的 **claimsMappingPolicy** 对象，则应用必须同意这两项授权。否则，将返回错误 `403 Forbidden`。

将来，任一权限都足以调用这两种方法。

## <a name="json-batching"></a>JSON 批处理

### <a name="nested-batches-are-not-supported"></a>不支持嵌套批处理

JSON 批处理请求中不得包含任何嵌套批处理请求。

### <a name="all-individual-requests-must-be-synchronous"></a>所有单个请求必须同步

批处理请求中包含的所有请求都必须同步执行。如果存在，将忽略 `respond-async` 首选项。

### <a name="transactional-processing-of-requests-is-not-supported"></a>不支持请求的事务处理

Microsoft Graph 当前不支持单个请求的事务处理。将忽略单个请求的 **atomicityGroup** 属性。

### <a name="uris-must-be-relative"></a>URI 必须相对

始终在批处理请求中指定相对的 URI。Microsoft Graph 将使用批处理 URL 中包含的版本终结点使这些 URL 绝对。

### <a name="batch-size-is-limited"></a>批处理大小受限

JSON 批处理请求目前限定为 20 个单独请求。 

* 根据批处理请求的 API 部分，基础服务会施加自己的限制，从而影响使用 Microsoft Graph 访问它们的应用程序。
* 批处理中的请求将根据限制单独进行评估，如果任何请求超过限制，则请求会失败，状态为 429。

有关更多详细信息，请访问 [限制和批处理](/graph/throttling#throttling-and-batching)。

### <a name="request-dependencies-are-limited"></a>请求依赖项受限

单独请求可以依赖其他单独请求。目前，请求只能依赖于单个其他请求，并且必须遵循下面的三种模式之一：

- 并行 - 没有单个请求在 **dependsOn** 属性中声明依赖项。
- 串行 - 所有单独请求都依赖于之前的单独请求。
- 相同 - 在 **dependsOn** 属性中声明依赖项的所有单个请求都声明相同的依赖项。 **Note**： 使用此模式发出的请求将按顺序运行。

随着 JSON 批处理技术日臻成熟，这些限制将会被取消。

## <a name="mail-outlook"></a>邮件 (Outlook)

### <a name="attaching-large-files-to-messages-with-delegated-permissions-can-fail"></a>将大文件附加到具有委派权限的邮件可能会失败
尝试[将大型文件附加](outlook-large-attachments.md)到共享或委派的邮箱中的 Outlook 邮件或事件时，具有委派权限的应用将返回 `HTTP 403 Forbidden`。 使用委派权限，仅当邮件或事件在已登录用户的邮箱中时，[createUploadSession](/graph/api/attachment-createuploadsession) 才会成功。

### <a name="the-comment-parameter-for-creating-a-draft-does-not-become-part-of-the-message-body"></a>用于创建草稿的注释参数不会成为邮件正文的一部分

用于创建答复或转发草稿的 **注释** 参数（[createReply](/graph/api/message-createreply)、[createReplyAll](/graph/api/message-createreplyall)、[createForward](/graph/api/message-createforward)）不会成为最终的邮件草稿正文的一部分。

### <a name="get-messages-returns-chats-in-microsoft-teams"></a>GET 消息返回 Microsoft Teams 中的聊天

在 v1.0 和 beta 终结点中，`GET /users/id/messages` 的响应包含出现在团队或频道范围外的用户的 Microsoft Teams 聊天。这些聊天消息的主体为“IM”。

## <a name="reports"></a>报告

### <a name="license-check-errors-for-azure-ad-activity-reports"></a>Azure AD 活动报告的许可证检查错误

当你拥有有效的 Azure AD Premium 许可证并调用 [directoryAudit](/graph/api/resources/directoryaudit)、[signIn](/graph/api/resources/signin) 或[预配 ](/graph/api/resources/provisioningobjectsummary)Azure AD 活动报告 API 时，你可能仍会遇到类似于以下内容的错误消息：

```json
{
    "error": {
        "code": "Authentication_RequestFromNonPremiumTenantOrB2CTenant",
        "message": "Neither tenant is B2C or tenant doesn't have premium license",
        "innerError": {
            "date": "2021-09-02T17:15:30",
            "request-id": "73badd94-c0ca-4b09-a3e6-20c1f5f9a307",
            "client-request-id": "73badd94-c0ca-4b09-a3e6-20c1f5f9a307"
        }
    }
}
```
在检索 [用户](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)资源的 **signInActivity** 属性时，也可能发生此错误；例如，`https://graph.microsoft.com/beta/users?$select=signInActivity`。

此错误是由于间歇性许可证检查失败造成的，我们正在努力解决此问题。 作为临时解决方法，请添加 **Directory.Read.All** 权限。 问题解决后，将不需要此临时解决方法。


## <a name="teamwork-microsoft-teams"></a>团队合作 (Microsoft Teams)

### <a name="unable-to-filter-team-members-by-roles"></a>无法按角色筛选团队成员
角色查询筛选器以及其他筛选器 `GET /teams/team-id/members?$filter=roles/any(r:r eq 'owner') and displayName eq 'dummy'` 可能不起作用。 服务可能使用 `BAD REQUEST` 响应。

### <a name="requests-to-filter-team-members-by-role-require-a-parameter"></a>按角色筛选团队成员的请求需要参数

所有按角色筛选团队成员的请求都要求在请求中使用 _skipToken_ 参数或 _top_ 参数，但不能同时使用两者。 如果两个参数都在请求中传递，则将忽略 _top_ 参数。

### <a name="some-properties-for-chat-members-might-be-missing-in-the-response-to-a-get-request"></a>GET 请求的响应中可能缺少聊天成员的某些属性
在某些情况下，聊天中`tenantId` / `email` / `displayName`成员的个人属性可能不会填充到请求`GET /chats/chat-id/members``GET /chats/chat-id/members/membership-id`中。

### <a name="properties-are-missing-in-the-list-of-teams-that-a-user-has-joined"></a>用户已加入的团队列表中缺少属性
目前，[我/joinedTeams](/graph/api/user-list-joinedteams) API 调用仅返回 [团队](/graph/api/resources/team)的 **id**、**displayName** 和 **说明** 属性。 若要获取所有属性，请使用[获取团队](/graph/api/team-get)操作。

### <a name="installation-of-apps-that-require-resource-specific-consent-permissions-is-not-supported"></a>不支持安装需要特定于资源的同意权限的应用
以下 API 调用不支持安装需要 [资源特定的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent) 权限的应用。
- [将应用添加到团队](/graph/api/team-post-installedapps.md)
- [升级团队中安装的应用](/graph/api/team-teamsappinstallation-upgrade.md)
- [将应用添加到聊天](/graph/api/chat-post-installedapps.md)
- [升级聊天中安装的应用](/graph/api/chat-teamsappinstallation-upgrade.md)

## <a name="users"></a>用户

### <a name="encode-number--symbols-in-userprincipalname"></a>对 userPrincipalName 中的数字符号 (#) 进行编码

通过 Azure AD B2B 添加的来宾用户的 **userPrincipalName** 通常包含数字字符 (#)。 如果对包含 # 符号的 **userPrincipalName** 使用 `$filter`，例如 `GET /users?$filter=userPrincipalName eq 'AdeleV_contoso.com#EXT#@fabrikam.com'`，将会返回 `400 Bad request` HTTP 错误响应。 若要按 **userPrincipalName** 进行筛选，请用其 UTF-8 等效字符 (`%23`) 对 # 字符进行编码，例如 `GET /users?$filter=userPrincipalName eq 'AdeleV_contoso.com%23EXT%23@fabrikam.com'`。

### <a name="access-to-user-resources-is-delayed-after-creation"></a>用户资源访问权限将在创建后延迟

可通过在用户实体上使用 POST 来即时创建用户。必须先向用户分配 Microsoft 365 许可证，然后用户才能访问 Microsoft 365 服务。尽管如此，由于服务具有分散特性，因此用户可能需要先等待 15 分钟，然后才能通过 Microsoft Graph API 使用文件、邮件和事件实体。在此期间，应用会收到一个 `404 Not Found` HTTP 错误响应。

### <a name="access-to-a-users-profile-photo-is-limited"></a>对用户的个人资料照片的访问受限

1. 只有当用户有邮箱时，才能读取和更新用户的个人资料照片。 在这种情况下，无法读取或更新照片会导致以下错误：

    ```html
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
    ``` 
2. 之前 *可能* 使用 **thumbnailPhoto** 属性（使用 Azure AD Graph API（已弃用），或通过 AD Connect 同步）存储的所有照片无法再通过 [用户](/graph/api/resources/user)资源的 Microsoft Graph **照片** 属性进行访问。
3. 目前，Azure AD B2C 租户不支持通过 Microsoft Graph API 的[profilePhoto 资源](/graph/api/resources/profilephoto)管理用户的照片。

### <a name="revoke-sign-in-sessions-returns-wrong-http-code"></a>调用登录会话返回了错误的 HTTP 代码

[用户: revokeSignInSessions API](/graph/api/user-revokesigninsessions) 返回 `204 No content` 响应表示成功调用；如果请求出现任何错误，则返回 HTTP 错误代码（4xx 或 5xx）。  但是，由于服务问题，此 API 会返回 `200 OK` 和始终为 `true` 的布尔值参数。  在此问题得到修复之前，可以将所有 2xx 返回代码看作此 API 成功。

### <a name="incomplete-objects-are-returned-when-using-getbyids-request"></a>使用 getByIds 请求时返回不完整的对象

使用[获取 ID 列表中的目录对象](/graph/api/directoryobject-getbyids)请求对象应返回完整对象。 但是，当前返回的 v1.0 端点上的[用户](/graph/api/resources/user)对象具有一组有限的属性。 作为临时解决方法，当您将该操作与 `$select` 查询选项结合使用时, 将返回更完整的[用户](/graph/api/resources/user)对象。 此行为不符合 OData 规范。 由于此行为可能在将来更新，因此仅在你提供 `$select=` 以及感兴趣的所有属性时，并且仅当此解决方法的未来重大更改可接受时，才使用此解决方法。

## <a name="query-parameters"></a>查询参数 

### <a name="some-limitations-apply-to-query-parameters"></a>查询参数存在一些限制

以下限制适用于查询参数：

* 不支持多个命名空间。
* 在用户、组、设备、服务主体和应用程序上，不支持对 `$ref` 执行 GET 请求和强制转换。
* `@odata.bind` 不受支持。这意味着无法在组上正确设置 **acceptedSenders** 或 **rejectedSenders** 导航属性。
* 使用极少的元数据时，非包容导航（如邮件）上不存在 `@odata.id`。
* `$expand`:
  * 最多返回 20 个对象。
  * 不支持 `@odata.nextLink`。
  * 不支持一级以上的扩展。
  * 不支持其他参数（`$filter`、`$select`）
* `$filter`:
  * `/attachments` 终结点不支持筛选器。 如果存在，将忽略 `$filter` 参数。
  * 不支持跨工作负载筛选。
* `$search`:
  * 全文搜索仅对实体子集（如邮件）可用。
  * 不支持跨工作负载搜索。
  * Azure AD B2C 租户不支持搜索。
* `$count`:
  * Azure AD B2C 租户不支持。
  * 在针对目录资源进行查询时使用 `$count=true` 查询字符串时， `@odata.count` 属性将仅出现在分页数据的第一页中。
* 请求中指定的查询参数可能会自行失败。 不支持的查询参数以及不支持的查询参数组合的情况就是如此。


## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis-deprecated"></a>功能仅在 Office 365 REST 或 Azure AD Graph API 中可用（已弃用）

某些功能尚未在 Microsoft Graph 中提供。 如果找不到所需的功能，请使用特定于终结点的 [Office 365 REST API](/previous-versions/office/office-365-api/)。 有关 Azure AD Graph，请参阅 [将 Azure Active Directory （Azure AD） Graph 应用迁移到 Microsoft Graph](./migrate-azure-ad-graph-overview.md)。