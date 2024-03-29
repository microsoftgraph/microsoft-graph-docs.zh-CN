---
title: Microsoft Graph 特定于服务的节流限制
description: 确定每个 Microsoft Graph 服务的限制，以应用最佳做法来管理应用程序中的节流。
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 9c0f4a057ae7cf1e729f44fabb0c98bde06cc500
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671415"
---
# <a name="microsoft-graph-service-specific-throttling-limits"></a>Microsoft Graph 特定于服务的节流限制

借助 Microsoft Graph，用户可访问[多个服务](overview-major-services.md)中的数据，如 Outlook 或 Azure Active Directory。 这些服务实施自己的限制，这些限制会影响使用 Microsoft Graph 访问它们的应用程序。

任何请求均可根据多个限制进行评估，具体取决于限制范围（所有租户中的每个应用、所有应用的每个租户、每个租户的每个应用等）、请求类型（GET、 POST、PATCH等）以及其他因素。 即将达到的第一个限制会触发阻止行为。 除了本节中描述的服务特定限制之外，还适用以下全局限制：

| 请求类型 | 所有租户中的每个应用  |
| ------------ | ------------------------ |
| 任何          | 每秒 2000 个请求 |

> [!NOTE]
> 此处所述的具体限制可能会发生更改。
>
> 在此部分中，术语 *租户* 是指安装应用程序的 Microsoft 365 组织。 对于单个租户应用程序，此租户可以与创建应用程序的租户相同，而对于 [多租户应用程序](/azure/active-directory/develop/setup-multi-tenant-app)，则可以不同。

### <a name="outlook-service-limits"></a>Outlook 服务限制

将评估每个应用 ID 和邮箱组合的 Outlook 服务限制。 换言之，上述限制适用于访问特定邮箱（用户或组）的特定应用。 如果一个邮箱的应用程序超过限制，不会影响访问另一个邮箱的功能。 下面的限制适用于公共云以及[区域云部署](./deployments.md)。

| 限制                                                      | 适用对象      |
|------------------------------------------------------------|-----------------|
| 10 分钟内的 10,000 个 API 请求                  | v1.0 和 beta 终结点 |
| 4 个并发请求                                      | v1.0 和 beta 终结点   |
| 30 秒内的 15 兆字节 (MB) 上传（PATCH、POST、PUT） | v1.0 和 beta 终结点   |

#### <a name="outlook-service-resources"></a>Outlook 服务资源

| API                                                      | 资源      |
|------------------------------------------------------------|-----------------|
| 搜索 API（预览版）                  | <li>[外部项（Microsoft 搜索）](/graph/api/resources/externalitem) |
| 配置文件 API                                      | <li>[照片](/graph/api/resources/profilephoto)   |
| 日历 API | <li>[事件](/graph/api/resources/event) <li> [eventMessage](/graph/api/resources/eventmessage) <li> [calendar](/graph/api/resources/calendar) <li>  [calendarGroup](/graph/api/resources/calendargroup) <li> [outlookCategory](/graph/api/resources/outlookcategory) <li> [attachment](/graph/api/resources/attachment) <li> [place（预览）](/graph/api/resources/place)   |
| 邮件 API                                      | <li>[邮件](/graph/api/resources/message) <li>  [邮件](/graph/api/resources/message) <li> [mailFolder](/graph/api/resources/mailfolder) <li> [mailSearchFolder](/graph/api/resources/mailsearchfolder) <li> [messageRule](/graph/api/resources/messagerule) <li> [outlookCategory](/graph/api/resources/outlookcategory) <li> [attachment](/graph/api/resources/attachment)|
| 个人联系人 API | <li>[contact](/graph/api/resources/contact) <li> [contactFolder](/graph/api/resources/contactfolder) <li> [outlookCategory](/graph/api/resources/outlookcategory)|
| 社交和工作场所智能 | <li>[person](/graph/api/resources/person) |
| 待办事项任务 API（预览版） | <li>[outlookTask](/graph/api/resources/outlooktask) <li> [outlookTaskFolder](/graph/api/resources/outlooktaskfolder) <li>[outlookTaskGroup](/graph/api/resources/outlooktaskgroup) <li> [outlookCategory](/graph/api/resources/outlookcategory) <li> [attachment](/graph/api/resources/attachment)|

### <a name="cloud-communication-service-limits"></a>云通信服务限制

| 资源      | 每个应用的限制    |
| -------------- | ------------ |
| [通话](/graph/api/resources/call) | 每月10,000 通通话和 100 通并发通话   |
| [会议信息](/graph/api/resources/meetinginfo)   | 每月每位用家会有 2000 则会议 |
| [状态](/graph/api/resources/presence)   | 平均每个租户每个应用在 30 秒的时间里 1500 个请求 |

### <a name="onenote-service-limits"></a>OneNote 服务限制

| 限制类型 | 每个用户的每个应用程序的限制（委派的上下文） | 每个应用程序的限制（仅应用程序上下文） |
| ------------ | ------- | ------- |
| 请求率 | 每 1 分钟 120 个请求和每 1 小时 400 个请求 | 每 1 分钟 240 个请求和每 1 小时 800 个请求 |
| 并发请求 | 5 个并发请求 | 20 个并发请求 |

上述限制适用于下列资源:

[!INCLUDE [Onenote throttling documentation](../includes/throttling-onenote.md)]

可在 [OneNote API 限制及避免方法](https://developer.microsoft.com/en-us/office/blogs/onenote-api-throttling-and-how-to-avoid-it/) 中找到有关最佳做法的附加信息。

> [!NOTE]
> 此前列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。

### <a name="project-rome-service-limits"></a>Project Rome 服务限制

| 请求类型 | 所有应用的每个用户的限制 |
| ------------ | --------------------------- |
| GET          | 每 5 分钟 400 个请求和每天 12000 个请求 |
| POST, PUT, PATCH, DELETE | 每 5 分钟 100 个请求和每天 8000 个请求 |

上述限制适用于下列资源:

- [activityHistoryItem](/graph/api/resources/activityhistoryitem)
- [userActivity](/graph/api/resources/useractivity)

### <a name="microsoft-teams-service-limits"></a>Microsoft Teams 服务限制

限制表示为每秒请求数 (rps)。

| Teams 请求类型                                   | 每个租户每个应用限制        | 所有租户中的每个应用限制      |
|------------------------------------------------------|---------------------------------|------------|
| GET team, channel, tab, installedApps, appCatalogs   | 30 rps                          | 600 rps |
| POST/PUT channel, tab, installedApps, appCatalogs    |  30 rps                         | 300 rps  |
| PATCH team, channel, tab, installedApps, appCatalogs |  30 rps                         | 300 rps  |
| DELETE channel, tab, installedApps, appCatalogs      |  15 rps                         | 150 rps  |
| GET /teams/```{team-id}```, joinedTeams              |  30 rps                         | 300 rps  |
| POST /teams | 10 rps | 100 rps  |
| PUT /groups/```{team-id}```/team, clone | 6 rps | 150 rps  |
| GET channel message  | 20 rps | 200 rps |
| GET 1:1/group chat message  | 20 rps | 200 rps |
| POST channel message | 50 rps | 500 rps |
| POST 1:1/group chat message | 20 rps | 200 rps |
| GET/teams/```{team-id}```/在以下路径下的日程安排和所有 API | 30 rps | 600 rps |
| POST, PATCH, PUT /teams/```{team-id}```/在以下路径下的日程安排和所有 API | 30 rps | 300 rps |
| DELETE /teams/```{team-id}```/在以下路径下的日程安排和所有 API | 15 rps | 150 rps |
| POST /teams/```{team-id}```/sendActivityNotification | 5 rps | 50 rps |
| POST /chats/```{chat-id}```/sendActivityNotification | 5 rps | 50 rps |
| POST /users/```{user-id}```/teamwork/sendActivityNotification | 5 rps | 50 rps |
| Microsoft Teams 的其他 GET API 调用              | 30 rps | 1500 rps |
| Microsoft Teams 的其他 API 调用              | 30 rps | 300 rps |

对于给定团队或频道，每个应用最多可发布 4 个请求。
每个应用每天最多可以将 3000 条消息发送到给定的频道。

另请参阅 [Microsoft Teams 限制](/graph/api/resources/teams-api-overview#microsoft-teams-limits)和[投票要求](/graph/api/resources/teams-api-overview#polling-requirements)。

[!INCLUDE [Teams throttling documentation](../includes/throttling-teams.md)]

### <a name="identity-and-access-service-limits"></a>身份和访问服务限制

本部分中的服务限制适用于以下实体：

[!INCLUDE [Identity and access throttling documentation](../includes/throttling-identity-and-access.md)]

#### <a name="pattern"></a>模式

限制基于令牌存储桶算法，后者通过添加各个请求的成本来实现。 然后将请求成本的总和与预定限制进行比较。 只有超出限制的请求才会被限制。 如果超出任何限制，则响应将为 `429 Too Many Requests`。 即使在服务处于重要负载或基于特定租户的数据量的情况下，也可能会收到 `429 Too Many Requests` 的响应，而不会达到以下限制。 下表列出了现有限制。

| 限制类型 | 资源单元配额 | 写入配额 |
| ---------- | ----------- | -------------- |
| 应用 + 租户对 | S：每 10 秒 3,500 个请求 <br/> M：每 10 秒 5,000 个请求 <br/> L：每 10 秒 8,000 个请求 | 每 2 分钟 30 秒 3,000 个请求 |
| 应用程序 | 每 20 秒 150,000 个请求  | 每 5 分钟 70,000 个请求|
| 租户 | 不适用 | 每 5 分钟 18,000 个请求 |

> [!NOTE]
> 应用程序 + 租户对限制因运行请求的租户中的用户数而异。 租户规模定义如下：S - 小于 50 个用户，M - 50 至 500 个用户之间，L - 500 个以上用户。

下表列出了基本请求费用。 未列出的任何请求的基础成本为 1。

| 操作 | 请求路径 | 基本资源单位成本 | 写入成本 |
| --------- | ------------ | ----------------- | ------------------ |
| GET | `applications` | 2 | 0 |
| GET | `applications/{id}/extensionProperties` | 2 | 0 |
| GET | `contracts` | 3 | 0 |
| POST | `directoryObjects/getByIds` |  3 | 0 |
| GET | `domains/{id}/domainNameReferences` | 4 | 0 |
| POST | `getObjectsById` | 3 | 0 |
| GET | `groups/{id}/members` | 3 | 0 |
| GET | `groups/{id}/transitiveMembers` | 5 | 0 |
| POST | `isMemberOf` | 4 | 0 |
| POST | `me/checkMemberGroups` | 4 | 0 |
| POST | `me/checkMemberObjects` | 4 | 0 |
| POST | `me/getMemberGroups` | 2 | 0 |
| POST | `me/getMemberObjects` | 2 | 0 |
| GET | `me/licenseDetails` | 2 | 0 |
| GET | `me/memberOf` | 2 | 0 |
| GET | `me/ownedObjects` | 2 | 0 |
| GET | `me/transitiveMemberOf` | 2 | 0 |
| GET | `oauth2PermissionGrants` | 2 | 0 |
| GET | `oauth2PermissionGrants/{id}` | 2 | 0 |
| GET | `servicePrincipals/{id}/appRoleAssignments` | 2 | 0 |
| GET | `subscribedSkus` | 3 | 0 |
| GET | `users` | 2 | 0 |
| GET | 表中未列出的任何身份路径 | 1 | 0 |
| POST | 表中未列出的任何身份路径 | 1 | 1 |
| PATCH | 表中未列出的任何身份路径 | 1 | 1 |
| PUT | 表中未列出的任何身份路径 | 1 | 1 |
| DELETE | 表中未列出的任何身份路径 | 1 | 1 |

> [!IMPORTANT]
> 
> 请求路径上的 POST、PATCH 和 DELETE `applications` 操作的成本取决于 **signInAudience** 类型。 对于`AzureADMyOrg`或`AzureADMultipleOrgs`**signInAudience** 的应用，每 5 分钟 70,000 个请求；而对于 **signInAudience** 为`AzureADandPersonalMicrosoftAccount`或`PersonalMicrosoftAccount`的应用，成本为每分钟 60 个请求。

影响请求费用的其他因素：

- 使用 `$select` 可将成本降低 1
- 使用 `$expand` 可将成本增加 1
- 使用值小于 20 的 `$top` 会使成本降低1
- 在 Azure AD B2C 租户中创建用户会将成本增加 4

> [!NOTE]
> 请求费用不能低于 1。 适用于从 `me/` 开始的请求路径的任何请求费用也适用于以 `users/{id | userPrincipalName}/`开头的等效请求。

#### <a name="additional-headers"></a>附加标题

##### <a name="request-headers"></a>请求标头

- **x-ms-throttle-priority** - 如果标头不存在或设置为任何其他值，则表示正常请求。 我们建议将优先级 `high` 用户启动的请求设置优先级。 此标头的值可以是以下值：
  - 低 - 指示请求的优先级较低。 限制此请求不会导致出现用户可见的故障。
  - 正常 - 如果未提供任何值，则为默认值。 表示请求是默认优先级。
  - 高 - 表示请求具有高优先级。 限制此请求会导致出现用户可见的故障。

> [!NOTE]
> 如果限制请求，将首先限制低优先级请求，其次限制普通优先级请求，最后限制高优先级请求。 使用优先级请求标头不会更改限制。

##### <a name="regular-responses-requests"></a>正常响应请求

- **x-ms-resource-unit** - 指示用于此请求的资源单位。值为正整数。
- **x-ms-throttle-limit-percentage** - 仅当应用程序消耗了超过其限制的 0.8 时才返回。 该值的范围是 0.8 到 1.8，是使用限制的百分比。 调用者可以使用该值设置警报并采取措施。

##### <a name="throttled-responses-requests"></a>受限制的响应请求

- **x-ms-throttle-scope** - eg. `Tenant_Application/ReadWrite/9a3d526c-b3c1-4479-ba74-197b5c5751ae/0785ef7c-2d7a-4542-b048-95bcab406e0b`. 指示采用下列格式 `<Scope>/<Limit>/<ApplicationId>/<TenantId|UserId|ResourceId>` 的限制范围：
  - 范围：（字符串，必填）
    - Tenant_Application - 当前应用程序对特定租户的所有请求。
    - 租户 - 当前租户的所有请求，与应用程序无关。
    - 应用程序 - 当前应用程序的所有请求。
  - 限制：（字符串、必填）
    - 读取：读取范围请求 (GET)
    - 写入：写入范围请求 (POST、PATCH、PUT、DELETE...)
    - ReadWrite：所有范围请求（任何）
  - ApplicationId （Guid、必填）
  - TenantId|UserId|ResourceId: (Guid、必填）
- **x-ms-throttle-information** - 指示限制的原因，可以有任何值（字符串）。 提供该值是为了进行诊断和故障排除，其中一些示例包括：
  - CPULimitExceeded - 限制因为超过 cpu 应用的限值。
  - WriteLimitExceeded - 限制因为超过写入限值。
  - ResourceUnitLimitExceeded - 限制因为超过已分配资源单位的限值。

### <a name="identity-and-access-reports-service-limits"></a>身份和访问报告服务限制

| 请求类型 |  每个租户每个应用限制 |
| ------------ | ------------------------ |
| 任何 | 每 10 秒 5 个请求 |

上述限制适用于下列资源:

[!INCLUDE [Azure AD identity and access reports throttling documentation](../includes/throttling-aad-reports.md)]

#### <a name="identity-and-access-reports-best-practices"></a>标识和访问报告最佳做法
当 Azure AD 在给定时间范围内从租户或应用接收过多调用时，Azure AD 报告 API 会受到限制。 如果服务响应时间过长，则调用也可能受到限制。 如果尽管应用了 [处理限制的最佳做法](throttling.md#best-practices-to-handle-throttling)，但请求仍然失败并出现 `429 Too Many Requests` 错误代码，请尝试减少返回的数据量。 首先尝试以下方法:
- 使用筛选器将查询定位到所需数据。 例如，如果只需要特定类型的事件或部分用户，请使用 `$filter` 和 `$select` 查询参数筛选出其他事件，从而减小响应对象的大小并减少限制风险。
- 如果需要大量 Azure AD 报告数据，请使用 **createdDateTime** 上的 `$filter` 以限制在单个调用中查询的登录事件数。 然后，循环访问下一个时间跨度，直到获得所需的所有记录。 例如，如果受到限制，则可以从请求 3 天数据的调用开始，并以较短的时间跨度循环访问，直到请求不再受到限制。
  
### <a name="information-protection-service-limits"></a>信息保护服务限制

以下限制适用于 `/informationProtection` 上的所有请求。

对于电子邮件，资源是唯一的网络消息 ID/收件人对。 例如，在 15 分钟内多次向同一个人提交具有相同邮件 ID 的电子邮件将触发下表中列出的每个资源限制的限制。 但是，每 15 分钟最多可以提交 150 封唯一电子邮件（租户限制）。

| 操作                 | 每个租户的使用限制                                            | 每个资源（电子邮件、URL、文件）的使用限制                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| POST                      | 每 15 分钟 150 个请求和每 24 小时 10000 个请求 | 每 15 分钟 1 个请求和每 24 小时 3 个请求 |

[!INCLUDE [Information protection throttling documentation](../includes/throttling-information-protection.md)]

### <a name="identity-protection-and-conditional-access-service-limits"></a>身份保护和条件访问服务限制

| 请求类型 | 所有应用的每个租户的使用限制 |
| ------------ | ------- |
| 任何 | 每秒1个请求 |

[!INCLUDE [Information protection throttling documentation](../includes/throttling-identityprotection-ca.md)]

> [!NOTE]
> 此前列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。

### <a name="insights-service-limits"></a>见解服务限制

以下限制适用于 `me/insights`或`users/{id}/insights` 上的所有请求。

| 限制                                                      | 适用对象      |
|------------------------------------------------------------|-----------------|
| 10 分钟内的 10,000 个 API 请求                  | v1.0 和 beta 终结点 |
| 4 个并发请求                                      | v1.0 和 beta 终结点   |

上述限制适用于下列资源:

- [people](/graph/api/resources/people)
- [sharedInsight](/graph/api/resources/sharedinsight)
- [trending](/graph/api/resources/trending)
- [usedInsight](/graph/api/resources/usedinsight)

### <a name="microsoft-graph-reports-service-limits"></a>Microsoft Graph 报告的服务限制

以下限制适用于 `/reports` 上的所有请求。

| 操作                 | 每个租户每个应用限制     | 所有应用的每个租户的使用限制 |
|---------------------------|------------------------------|----------------------------|
| 任何请求（CSV）         | 每10分钟14个请求   | 每10分钟40个请求 |
| 任何请求（JSON、beta）  | 每10分钟100个请求  | 不适用                        |

上述限制分别适用于每个报告 API。例如，在 10 分钟内分别有对 Microsoft Teams 用户活动报告 API 的请求及对 Outlook 用户活动报告 API 的请求，将分别被视为 14 个请求中的 1 个请求，而不是 14 个请求中的 2 个请求。

上述限制适用于所有 [使用情况报表](/graph/api/resources/report) 资源。

### <a name="invitation-manager-service-limits"></a>邀请管理器服务限制

以下限制适用于 `/invitations` 上的所有请求。

| 操作                 | 所有应用的每个租户的使用限制 |
|---------------------------|------------------------------|
| 任何操作             | 每 5 秒 150 个请求   |

### <a name="security-detections-and-incidents-service-limits"></a>安全检测和事件服务限制

以下限制适用于 `/security` 上的所有请求。

| 操作                  | 每个租户每个应用限制     |
|----------------------------|------------------------------|
| `alert`、`securityActions`、`secureScore` 上的任何操作 | 每分钟 150 个请求      |
| `tiIndicator` 上的任何操作 | 每分钟 1000 个请求 |
| `secureScore` 或 `secureScorecontrolProfile` 上的任何操作 | 10 分钟内的 10,000 个 API 请求 |
| `secureScore` 或 `secureScorecontrolProfile` 上的任何操作 | 4 个并发请求 |

### <a name="open-and-schema-extensions-service-limits"></a>开放和架构扩展服务限制

| 请求类型 | 每个租户每个应用限制 |
| ------------ | ------------------------ |
| 任何          | 每 10 秒 455 个请求 |

上述限制适用于下列资源：[!INCLUDE [Open and schema extensions throttling documentation](../includes/throttling-extensions.md)]

### <a name="files-and-lists-service-limits"></a>文件和列表服务限制

有关 OneDrive、OneDrive for Business 和 SharePoint Online 的服务限制，请参阅 [避免在 SharePoint Online 中受到限制或阻止](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)。

上述信息适用于以下资源：

[!INCLUDE [Files and lists throttling documentation](../includes/throttling-files-and-lists.md)]

### <a name="tasks-and-plans-service-limits"></a>任务和计划服务限制

Planner 的服务限制不可用。

上述信息适用于以下资源：[!INCLUDE [Tasks and plans throttling documentation](../includes/throttling-tasks-and-plans.md)]

### <a name="identity-and-access-data-policy-operation-service-limits"></a>身份和访问数据策略操作服务限制

| 请求类型 | 每个租户的使用限制 |
| ------------ | ---------------- |
| 发布于 `exportPersonalData` | 每天 1000 个针对任何主题的请求，每个主题每天 100 个请求 |
| 任何其他请求 | 每分钟 10000 个请求 |

上述限制适用于下列资源：

- [dataPolicyOperation](/graph/api/resources/datapolicyoperation)

> [!NOTE]
> 此前列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a>教育版服务限制

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a>Excel 服务限制

有关 Excel 服务限制的说明和最佳实践，请参阅 [减少限制错误](workbook-best-practice.md#reduce-throttling-errors)。 此外，还存在以下限制。
  
[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-providers-service-limits"></a>身份提供程序的服务限制

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a>Intune服务限制

[!INCLUDE [Intune  tunnel throttling documentation](../includes/throttling-intune-throttling-tunnel.md)]
[!INCLUDE [Intune android for work throttling documentation](../includes/throttling-intune-android-for-work.md)]
[!INCLUDE [Intune applications throttling documentation](../includes/throttling-intune-applications.md)]
[!INCLUDE [Intune auditing throttling documentation](../includes/throttling-intune-auditing.md)]
[!INCLUDE [Intune books throttling documentation](../includes/throttling-intune-books.md)]
[!INCLUDE [Intune bundles throttling documentation](../includes/throttling-intune-bundles.md)]
[!INCLUDE [Intune chromebook sync throttling documentation](../includes/throttling-intune-chromebook-sync.md)]
[!INCLUDE [Intune company terms throttling documentation](../includes/throttling-intune-company-terms.md)]
[!INCLUDE [Intune device config v2 throttling documentation](../includes/throttling-intune-device-config-v2.md)]
[!INCLUDE [Intune device configuration throttling documentation](../includes/throttling-intune-device-configuration.md)]
[!INCLUDE [Intune device enrollment throttling documentation](../includes/throttling-intune-device-enrollment.md)]
[!INCLUDE [Intune device intent throttling documentation](../includes/throttling-intune-device-intent.md)]
[!INCLUDE [Intune devices throttling documentation](../includes/throttling-intune-devices.md)]
[!INCLUDE [Intune endpoint protection throttling documentation](../includes/throttling-intune-endpoint-protection.md)]
[!INCLUDE [Intune enrollment throttling documentation](../includes/throttling-intune-enrollment.md)]
[!INCLUDE [Intune fencing throttling documentation](../includes/throttling-intune-fencing.md)]
[!INCLUDE [Intune GPAnalytics throttling documentation](../includes/throttling-intune-gpanalytics.md)]
[!INCLUDE [Intune managed applications throttling documentation](../includes/throttling-intune-managed-applications.md)]
[!INCLUDE [Intune notifications throttling documentation](../includes/throttling-intune-notifications.md)]
[!INCLUDE [Intune ODJ throttling documentation](../includes/throttling-intune-odj.md)]
[!INCLUDE [Intune partner integration throttling documentation](../includes/throttling-intune-partner-integration.md)]
[!INCLUDE [Intune rbac throttling documentation](../includes/throttling-intune-rbac.md)]
[!INCLUDE [Intune remote assistance throttling documentation](../includes/throttling-intune-remote-assistance.md)]
[!INCLUDE [Intune telephony throttling documentation](../includes/throttling-intune-telephony.md)]
[!INCLUDE [Intune TEM throttling documentation](../includes/throttling-intune-tem.md)]
[!INCLUDE [Intune troubleshooting throttling documentation](../includes/throttling-intune-troubleshooting.md)]
[!INCLUDE [Intune unlock throttling documentation](../includes/throttling-intune-unlock.md)]
[!INCLUDE [Intune updates throttling documentation](../includes/throttling-intune-updates.md)]
[!INCLUDE [Intune wip throttling documentation](../includes/throttling-intune-wip.md)]

### <a name="multi-service-limits"></a>多服务限制

[!INCLUDE [Multi tenant platform throttling documentation](../includes/throttling-multi-tenant-platform.md)]

### <a name="skype-service-limits"></a>Skype 服务限制

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a>订阅服务

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->

### <a name="assignment-service-limits"></a>作业服务限制

下列的限制适用于关于作业服务 API 的请求:

| 请求类型                 | 每个租户每个应用限制     | 所有应用的每个租户的使用限制 |
|---------------------------|------------------------------|----------------------------|
| 任何         | 每 10 秒 500 个请求   | 每 10 秒 1000 个请求
|任何          | 每 3600 秒 15000 个请求|每 3600 秒 30000 个请求|
| 获取/作业  | 每 10 秒 50 个请求 | 每 10 秒 150 个请求 |

上述限制适用于下列资源：

- [educationAssignment](/graph/api/resources/educationassignment)
- [educationSubmission](/graph/api/resources/educationsubmission)
- [trending](/graph/api/resources/trending)
- [educationResource](/graph/api/resources/educationresource)


### <a name="service-communications-service-limits"></a>服务通信服务限制
以下限制适用于`/admin/serviceAnnouncement/`下任何类型的服务通信请求。

| 请求类型 |  每个租户每个应用限制 |
| ------------ | ------------------------ |
| 任何 | 每 60 秒 240 个请求 |
|任何 | 每小时 800 个请求 |

