---
title: Microsoft Graph 限制指南
description: 限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 82abc2a316fc3a5d14902089802862165081fada
ms.sourcegitcommit: 10d9f4c2cee192bd80984d48cabba63b47c54551
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2021
ms.locfileid: "53578942"
---
# <a name="microsoft-graph-throttling-guidance"></a>Microsoft Graph 限制指南

限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。

根据该方案，执行的限制会有所不同。例如，如果你正在执行大量的写入操作，限制的可能性会比仅执行读取时要高。

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a>在限制时，会发生什么情况？
<!-- markdownlint-enable MD026 -->

超出限制阈值后，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步的请求。发生限制时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），同时请求失败。在失败的请求的响应标头中返回建议的等待时间。限制行为取决于请求的类型和数量。例如，如果你有大量的请求，则所有请求类型受限。阈值限制根据请求类型而有所不同。因此，你可能会遇到这样一种场景，在场景中，写入被限制，但仍允许读取。

## <a name="common-throttling-scenarios"></a>常见的限制场景

客户端受限的最常见原因包括：

- 来自租户中所有应用程序的请求太多。
- 来自所有租户中特定应用程序的请求太多。

## <a name="sample-response"></a>示例响应

每当超出限制阈值时，Microsoft Graph 都会提供与此类似的响应。

```http
HTTP/1.1 429 Too Many Requests
Content-Type: application/json
Retry-After: 2.128

{
  "error": {
    "code": "TooManyRequests",
    "innerError": {
      "code": "429",
      "date": "2020-08-18T12:51:51",
      "message": "Please retry after",
      "request-id": "94fb3b52-452a-4535-a601-69e0a90e3aa2",
      "status": "429"
    },
    "message": "Please retry again later."
  }
}
```

## <a name="best-practices-to-handle-throttling"></a>处理限制的最佳实践

以下是处理限制的最佳做法：

- 减少每个请求的操作数量。
- 减少调用频率。
- 不要立即重试，因为所有请求都会计入使用限制。

进行错误处理时，使用 HTTP 错误代码 429 检测限制。失败的响应包括 `Retry-After` 响应标头。使用 `Retry-After` 延迟回退请求是从限制中恢复的最快速的方式，因为 Microsoft Graph 会在客户端受限时继续记录资源使用状况。

1. 等待 `Retry-After` 标头中指定的秒数。
2. 请重试请求。
3. 如果请求再次失败，并显示 429 错误代码，则表示你仍然受限。继续使用建议的 `Retry-After` 延迟并重试请求直到成功。

除非有说明，否则[服务特定限制](#service-specific-limits)部分中所述的所有资源和 API 均提供 `Retry-After` 标头。

有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](/azure/architecture/patterns/throttling)。

> [!NOTE]
> 如果响应未提供 `Retry-After` 标头，我们建议实施指数退避重试策略。 构建大型应用程序时，还可以实现[更高级的模式](/azure/architecture/patterns/category/resiliency)。
>
> Microsoft Graph SDK 已实施依赖于 `Retry-After` 标头或默认为指数退避重试策略的处理程序。

## <a name="best-practices-to-avoid-throttling"></a>避免限制的最佳做法

如持续轮询资源以检查更新以及定期扫描资源集合以检查新资源或已删除资源之类的编程模式，更有可能导致应用程序受到限制并降低整体性能。 如果可用，改为使用[更改跟踪](delta-query-overview.md)并[更改通知](webhooks.md)。

>[!NOTE]
>[大规模发现文件和检测更改的最佳做法](/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online)详细介绍最佳做法。

## <a name="throttling-and-batching"></a>限制和批处理

[JSON 批处理](./json-batching.md)使你能够通过将多个请求合并为单个 JSON 对象来优化应用程序。 批次中的请求将根据限制进行单独评估，如果任何请求超出限制，则它将失败，并出现 `status` `429` 以及类似于上述内容的错误。 批次本身失败，状态代码为 `424`（失败的相关性）。 多个请求可能会在单个批次中受到限制。 应使用 JSON 内容的 `retry-after` 响应标头中提供的值，尝试批次中每个失败的请求。 你可以在最长 `retry-after` 值之后重试新批次中所有失败的请求。

如果在受限制请求未经批处理时，SDK 自动重试这些请求，则不会自动重试属于批次的受限制请求。

## <a name="service-specific-limits"></a>服务特定限制

借助 Microsoft Graph，用户可访问[多个服务](overview-major-services.md)中的数据，如 Outlook 或 Azure Active Directory。 这些服务实施自己的限制，这些限制会影响使用 Microsoft Graph 访问它们的应用程序。

任何请求均可根据多个限制进行评估，具体取决于限制范围（所有租户中的每个应用、所有应用的每个租户、每个租户的每个应用等）、请求类型（GET、 POST、PATCH等）以及其他因素。 即将达到的第一个限制会触发阻止行为。 除了本节中描述的服务特定限制之外，还适用以下全局限制：

| 请求类型 | 所有租户中的每个应用  |
| ------------ | ------------------------ |
| 任何          | 每秒 2000 个请求 |

> [!NOTE]
> 此处所述的具体限制可能会发生更改。

> **备注** 在本节中，*租户* 此术语是指指安装应用程序的 Microsoft 365 组织。 对于单个租户应用程序，这个租户可以与创建应用程序的租户相同，对于[多租户应用程序](/azure/active-directory/develop/setup-multi-tenant-app)，这个租户可以不同。

### <a name="outlook-service-limits"></a>Outlook 服务限制

将评估每个应用 ID 和邮箱组合的 Outlook 服务限制。 换言之，上述限制适用于访问特定邮箱（用户或组）的特定应用。 如果一个邮箱的应用程序超过限制，不会影响访问另一个邮箱的功能。 下面的限制适用于公共云以及[区域云部署](./deployments.md)。

| 限制                                                      | 适用对象      |
|------------------------------------------------------------|-----------------|
| 10 分钟内的 10,000 个 API 请求                  | v1.0 和 beta 终结点 |
| 4 个并发请求                                      | v1.0 和 beta 终结点   |
| 30 秒内的 15 兆字节 (MB) 上传（PATCH、POST、PUT） | v1.0 和 beta 终结点   |

#### <a name="outlook-service-resources"></a>Outlook 服务资源

Outlook 服务提供以下资源。

##### <a name="search-api-resources-preview"></a>搜索 API 资源（预览版）

- [外部项（Microsoft 搜索）](/graph/api/resources/externalitem?view=graph-rest-beta)

##### <a name="profile-api-resources"></a>配置文件 API 资源

- [照片](/graph/api/resources/profilephoto?view=graph-rest-1.0)

##### <a name="calendar-api-resources"></a>日历 API 资源

- [event](/graph/api/resources/event)
- [eventMessage](/graph/api/resources/eventmessage)
- [calendar](/graph/api/resources/calendar)
- [calendarGroup](/graph/api/resources/calendargroup)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)
- [place（预览）](/graph/api/resources/place)

##### <a name="mail-api-resources"></a>邮件 API 资源

- [message](/graph/api/resources/message)
- [mailFolder](/graph/api/resources/mailfolder)
- [mailSearchFolder](/graph/api/resources/mailsearchfolder)
- [messageRule](/graph/api/resources/messagerule)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a>个人联系人 API 资源

- [contact](/graph/api/resources/contact)
- [contactFolder](/graph/api/resources/contactfolder)
- [outlookCategory](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a>社交和工作区智能资源

- [person](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a>待办任务 API（预览）资源

- [outlookTask](/graph/api/resources/outlooktask)
- [outlookTaskFolder](/graph/api/resources/outlooktaskfolder)
- [outlookTaskGroup](/graph/api/resources/outlooktaskgroup)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a>云通信服务限制

| 资源      | 每个应用的限制    |
| -------------- | ------------ |
| [通话](/graph/api/resources/call) | 每月10,000 通通话和 100 通并发通话   |
| [会议信息](/graph/api/resources/meetinginfo)   | 每月每位用家会有 2000 则会议 |
| [状态](/graph/api/resources/presence)（预览版）   | 平均每个租户每个应用在 30 秒的时间里 1500 个请求 |

### <a name="onenote-service-limits"></a>OneNote 服务限制

| 限制类型 | 每个用户的每个应用程序的限制（委派的上下文） | 每个应用程序的限制（仅应用程序上下文） |
| ------------ | ------- | ------- |
| 请求率 | 每 1 分钟 120 个请求和每 1 小时 400 个请求 | 每 1 分钟 240 个请求和每 1 小时 800 个请求 |
| 并发请求 | 5 个并发请求 | 20 个并发请求 |

上述限制适用于下列资源:  
onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation

可在 [OneNote API 限制及避免方法](https://developer.microsoft.com/zh-CN/office/blogs/onenote-api-throttling-and-how-to-avoid-it/) 中找到有关最佳做法的附加信息。  

> **注意：** 上面列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。

### <a name="project-rome-service-limits"></a>Project Rome 服务限制

| 请求类型 | 所有应用的每个用户的限制 |
| ------------ | --------------------------- |
| GET          | 每 5 分钟 400 个请求和每天 12000 个请求 |
| POST, PUT, PATCH, DELETE | 每 5 分钟 100 个请求和每天 8000 个请求 |

上述限制适用于下列资源:  
activityHistoryItem、userActivity

### <a name="microsoft-teams-service-limits"></a>Microsoft Teams 服务限制

限制表示为每秒请求数 (rps)。

| Teams 请求类型                                   | 每个租户每个应用限制        | 所有租户中的每个应用限制      |
|------------------------------------------------------|---------------------------------|------------|
| Microsoft Teams 的任何图形 API 调用              | 每 10 秒 15000 个请求 | 不适用 |
| GET team, channel, tab, installedApps, appCatalogs   | 60 rps                          | 600 rps |
| POST/PUT channel, tab, installedApps, appCatalogs    |  30 rps                         | 300 rps  |
| PATCH team, channel, tab, installedApps, appCatalogs |  30 rps                         | 300 rps  |
| DELETE channel, tab, installedApps, appCatalogs      |  15 rps                         | 150 rps  |
| GET /teams/```{team-id}```, joinedTeams              |  30 rps                         | 300 rps  |
| POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone | 6 rps | 150 rps  |
| GET channel message  | 5 rps | 100 rps |
| GET 1:1/group chat message  | 3 rps | 30 rps |
| POST channel message | 2 rps | 20 rps |
| POST 1:1/group chat message | 2 rps | 20 rps |
| GET/teams/```{team-id}```/在以下路径下的日程安排和所有 API | 60 rps | 600 rps |
| POST, PATCH, PUT /teams/```{team-id}```/在以下路径下的日程安排和所有 API | 30 rps | 300 rps |
| DELETE /teams/```{team-id}```/在以下路径下的日程安排和所有 API | 15 rps | 150 rps |

对于给定团队或频道，每个应用最多可发布 4 个请求。
每个应用每天最多可以将 3000 条消息发送到给定的频道。

另请参阅 [Microsoft Teams 限制](/graph/api/resources/teams-api-overview#microsoft-teams-limits)和[投票要求](/graph/api/resources/teams-api-overview#polling-requirements)。

上述限制适用于下列资源:  
aadUserConversationMember、appCatalogs、changeTrackedEntity、channel、chatMessage、chatMessageHostedContent、conversationMember、offerShiftRequest、openShift、openShiftChangeRequest、schedule、scheduleChangeRequest、schedulingGroup、shift、shiftPreferences、swapShiftsChangeRequest、team、teamsApp、teamsAppDefinition、teamsAppInstallation、teamsAsyncOperation、teamsTab、teamsTemplate、teamwork、timeOff、timeOffReason、timeOffRequest、userSettings、workforceIntegration。

### <a name="identity-and-access-service-limits"></a>身份和访问服务限制

这些服务限制适用于以下实体：

- [目录对象](/graph/api/resources/directoryobject)
- [扩展属性](/graph/api/resources/extensionproperty)
- [管理单元](/graph/api/resources/administrativeunit)
- [应用程序](/graph/api/resources/application)
- [应用角色分配](/graph/api/resources/approleassignment)
- [基于证书的身份配置](/graph/api/resources/certificatebasedauthconfiguration)
- [组织联系人](/graph/api/resources/orgcontact)
- [Device](/graph/api/resources/device)
- [目录对象合作伙伴参考](/graph/api/resources/directoryobjectpartnerreference)
- [目录角色](/graph/api/resources/directoryrole)
- [目录角色模板](/graph/api/resources/directoryroletemplate)
- [域](/graph/api/resources/domain)
- [域 dns 记录](/graph/api/resources/domaindnsrecord)
- [域 dns cname 记录](/graph/api/resources/domaindnscnamerecord)
- [域 dns mx 记录](/graph/api/resources/domaindnsmxrecord)
- [域 dns srv 记录](/graph/api/resources/domaindnssrvrecord)
- [域 dns txt 记录](/graph/api/resources/domaindnstxtrecord)
- [域 dns 不可用记录](/graph/api/resources/domaindnsunavailablerecord)
- [终结点](/graph/api/resources/endpoint)
- [扩展属性](/graph/api/resources/extensionproperty)
- [许可证详细信息](/graph/api/resources/licensedetails)
- [组](/graph/api/resources/group)
- [基于活动的超时策略](/graph/api/resources/activitybasedtimeoutpolicy)
- [声明映射策略](/graph/api/resources/claimsmappingpolicy)
- [主领域发现策略](/graph/api/resources/homerealmdiscoverypolicy)
- [令牌颁发策略](/graph/api/resources/tokenissuancepolicy)
- [令牌生存期策略](/graph/api/resources/tokenlifetimepolicy)
- [策略基础](/graph/api/resources/policybase)
- [Sts 策略](/graph/api/resources/stspolicy)
- [合同](/graph/api/resources/contract)
- [服务主体](/graph/api/resources/serviceprincipal)
- [订阅的 SKU](/graph/api/resources/subscribedsku)
- [Oauth2 权限授予](/graph/api/resources/oauth2permissiongrant)
- [组织](/graph/api/resources/organization)
- [用户](/graph/api/resources/user)
- [组设置](/graph/api/resources/groupsetting)
- [组设置模板](/graph/api/resources/groupsettingtemplate)

#### <a name="pattern"></a>模式

限制基于令牌存储桶算法，后者通过添加各个请求的成本来实现。 然后将请求成本的总和与预定限制进行比较。 只有超出限制的请求才会被限制。 如果超出任何限制，则响应将为 `429 Too Many Requests`。 即使在服务处于重要负载或基于特定租户的数据量的情况下，也可能会收到 `429 Too Many Requests` 的响应，而不会达到以下限制。 下表列出了现有限制。

| 限制类型 | 资源单元配额 | 写入配额 |
| ---------- | ----------- | -------------- |
| 应用 + 租户对 | S：3500，M:5000，L:8000 每 10 秒钟 | 每 2 分钟 30 秒 3000 |
| 应用程序 | 每 20 秒 150,000  | 每 5 分钟 70,000 |
| 租户 | 不适用 | 每 5 分钟 18000 |

> **注意**：应用程序 + 租户对限制因租户请求中运行的用户数而异。 租户规模定义如下：S - 小于 50 个用户，M - 50 至 500 个用户之间，L - 500 个以上用户。

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

影响请求费用的其他因素：

- 使用 `$select` 可将成本降低 1
- 使用 `$expand` 可将成本增加 1
- 使用值小于 20 的 `$top` 会使成本降低1

> **注意：** 请求费用不能低于 1。 适用于从 `me/` 开始的请求路径的任何请求费用也适用于以 `users/{id | userPrincipalName}/`开头的等效请求。

#### <a name="additional-headers"></a>附加标题

##### <a name="request-headers"></a>请求标头

- **x-ms-throttle-priority** - 如果标头不存在或设置为任何其他值，则表示正常请求。 我们建议将优先级 `high` 用户启动的请求设置优先级。 此标头的值可以是以下值：
  - 低 - 指示请求的优先级较低。 限制此请求不会导致出现用户可见的故障。
  - 正常 - 如果未提供任何值，则为默认值。 表示请求是默认优先级。
  - 高 - 表示请求具有高优先级。 限制此请求会导致出现用户可见的故障。

> **注意**：如果限制请求，则首先限制低优先级请求，其次限制正常优先级请求，最后限制高优先级请求。 使用优先级请求标头不会更改限制。

##### <a name="regular-responses-requests"></a>正常响应请求

- **x-ms-resource-unit** - 指示用于此请求的资源单位。 值为正整数。
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

### <a name="information-protection"></a>信息保护

以下限制适用于 `/informationProtection` 上的所有请求。

| 操作                 | 每个租户的使用限制                                            | 每个资源（电子邮件、URL、文件）的使用限制                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| POST                      | 每 15 分钟 150 个请求和每 24 小时 10000 个请求 | 每 15 分钟 1 个请求和每 24 小时 3 个请求 |

上述限制适用于下列资源:  
threatAssessmentRequest、threatAssessmentResult、mailAssessmentRequest、emailFileAssessmentRequest、fileAssessmentRequest、urlAssessmentRequest。

### <a name="identity-protection-and-conditional-access-service-limits"></a>身份保护和条件访问服务限制

| 请求类型 | 所有应用的每个租户的使用限制 |
| ------------ | ------- |
| 任何 | 每秒1个请求 |

上述限制适用于下列资源:  
riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.

> **注意：** 上面列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。

### <a name="insights-service-limits"></a>见解服务限制

以下限制适用于 `me/insights`或`users/{id}/insights` 上的所有请求。

| 限制                                                      | 适用对象      |
|------------------------------------------------------------|-----------------|
| 10 分钟内的 10,000 个 API 请求                  | v1.0 和 beta 终结点 |
| 4 个并发请求                                      | v1.0 和 beta 终结点   |

上述限制适用于下列资源:  
people、trending、usedinsight、sharedInsight。

### <a name="microsoft-graph-reports-service-limits"></a>Microsoft Graph 报告的服务限制

以下限制适用于 `/reports` 上的所有请求。

| 操作                 | 每个租户每个应用限制     | 所有应用的每个租户的使用限制 |
|---------------------------|------------------------------|----------------------------|
| 任何请求（CSV）         | 每10分钟14个请求   | 每10分钟40个请求 |
| 任何请求（JSON、beta）  | 每10分钟100个请求  | 不适用                        |

上述限制分别适用于每个报表 API。 例如，在 10 分钟内分别有对 Microsoft Teams 用户活动报告 API 的请求及对 Outlook 用户活动报告 API 的请求，将分别被视为 14 个请求中的 1 个请求，而不是 14 个请求中的 2 个请求。

上述限制适用于 **报告** 资源。  

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

上述限制适用于以下资源：openTypeExtension、schemaExtension、administrativeUnit、合同、设备、事件、组、消息、组织、帖子和用户。

### <a name="files-and-lists-service-limits"></a>文件和列表服务限制

OneDrive、OneDrive for Business 和 SharePoint Online 的服务限制不可用。 有关详细信息，请参阅[为什么不能告诉我确切的限制？](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits)。

上述信息适用于以下资源：  
baseItem、baseItemVersion、columnDefinition、columnLink、contentType、drive、driveItem、driveItemVersion、fieldValueSet、itemActivity、itemActivityStat、itemAnalytics、list、listItem、listItemVersion、permission、sharedDriveItem、site 和 thumbnailSet。

### <a name="tasks-and-plans-service-limits"></a>任务和计划服务限制

Planner 的服务限制不可用。

上述信息适用于以下资源：  
planner、plannerAssignedToTaskBoardTaskFormat、plannerBucket、plannerBucketTaskBoardTaskFormat、plannerGroup、plannerPlan、plannerPlanDetails、plannerProgressTaskBoardTaskFormat、plannerTask、plannerTaskDetails 和 plannerUser。

### <a name="identity-and-access-data-policy-operation-service-limits"></a>身份和访问数据策略操作服务限制

| 请求类型 | 每个租户的使用限制 |
| ------------ | ---------------- |
| 发布于 `exportPersonalData` | 每天 1000 个针对任何主题的请求，每个主题每天 100 个请求 |
| 任何其他请求 | 每分钟 10000 个请求 |

上述限制适用于下列资源：dataPolicyOperation。

> **注意：** 上面列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a>教育版服务限制

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a>Excel 服务限制

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
[!INCLUDE [Intune device config V2 throttling documentation](../includes/throttling-intune-device-config-v2.md)]
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
[!INCLUDE [Intune reporting throttling documentation](../includes/throttling-intune-reporting.md)]
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
| 任何         | 每 10 秒 5000 个请求   | 每 10 秒 15000 个请求 |
| 获取/作业  | 每 10 秒 50 个请求 | 每 10 秒 150 个请求 |  

前面的限制适用于以下资源：[educationAssignment](/graph/api/resources/educationassignment?view=graph-rest)
[educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest)
[educationResource](/graph/api/resources/educationresource?view=graph-rest)
