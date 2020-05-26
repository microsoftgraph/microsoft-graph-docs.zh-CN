---
title: Microsoft Graph 限制指南
description: 限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: d33ac4612f4fe3934c53235360626dac1393ab21
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44215785"
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

## <a name="best-practices-to-handle-throttling"></a>处理限制的最佳实践

以下是处理限制的最佳做法：

- 减少每个请求的操作数量。
- 减少调用频率。
- 不要立即重试，因为所有请求都会计入使用限制。

进行错误处理时，使用 HTTP 错误代码 429 检测限制。失败的响应包括 `Retry-After` 响应标头。使用 `Retry-After` 延迟回退请求是从限制中恢复的最快速的方式，因为 Microsoft Graph 会在客户端受限时继续记录资源使用状况。

1. 等待 `Retry-After` 标头中指定的秒数。
2. 请重试请求。
3. 如果请求再次失败，并显示 429 错误代码，则表示你仍然受限。继续使用建议的 `Retry-After` 延迟并重试请求直到成功。

下列资源目前提供 `Retry-After` 标头：

- [用户](/graph/api/resources/user?view=graph-rest-1.0)
- [照片](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [邮件](/graph/api/resources/message?view=graph-rest-1.0)
- [日历（用户和组）](/graph/api/resources/event?view=graph-rest-1.0)
- [联系人](/graph/api/resources/contact?view=graph-rest-1.0)
- [附件](/graph/api/resources/attachment?view=graph-rest-1.0)
- [组对话](/graph/api/resources/conversation?view=graph-rest-1.0)
- [人员和社交活动](/graph/api/resources/social-overview?view=graph-rest-beta)
- [Drive (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0)
- [外部项（Microsoft 搜索）](/graph/api/resources/externalitem?view=graph-rest-beta)

有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](https://docs.microsoft.com/azure/architecture/patterns/throttling)。

> [!NOTE]
> 如果响应未提供 `Retry-After` 标头，我们建议实施指数退避重试策略。 构建大型应用程序时，还可以实现[更高级的模式](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency)。
>
> Microsoft Graph SDK 已实施依赖于 `Retry-After` 标头或默认为指数退避重试策略的处理程序。

## <a name="best-practices-to-avoid-throttling"></a>避免限制的最佳做法

如持续轮询资源以检查更新以及定期扫描资源集合以检查新资源或已删除资源之类的编程模式，更有可能导致应用程序受到限制并降低整体性能。 如果可用，改为使用[更改跟踪](delta-query-overview.md)并[更改通知](webhooks.md)。

>[!NOTE]
>[大规模发现文件和检测更改的最佳做法](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online)详细介绍最佳做法。

## <a name="service-specific-limits"></a>服务特定限制

借助 Microsoft Graph，用户可访问[多个服务](overview-major-services.md)中的数据，如 Outlook 或 Azure Active Directory。 这些服务实施自己的限制，这些限制会影响使用 Microsoft Graph 访问它们的应用程序。

> [!NOTE]
> 此处所述的具体限制可能会发生更改。

### <a name="outlook-service-limits"></a>Outlook 服务限制

将评估每个应用 ID 和邮箱组合的 Outlook 服务限制。 换言之，上述限制适用于访问特定邮箱（用户或组）的特定应用。 如果一个邮箱的应用程序超过限制，不会影响访问另一个邮箱的功能。

| 限制                                                      | 适用对象      |
|------------------------------------------------------------|-----------------|
| 10 分钟内的 10,000 个 API 请求                  | v1.0 和 beta 终结点 |
| 4 个并发请求                                      | Beta 终结点   |
| 30 秒内的 15 兆位上传（PATCH、POST、PUT） | Beta 终结点   |

#### <a name="outlook-service-resources"></a>Outlook 服务资源

Outlook 服务提供以下资源。

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

对于给定团队或频道，每个应用最多可发布 4 个请求。
每个应用每天最多可以将 3000 条消息发送到给定的频道。

另请参阅 [Microsoft Teams 限制](/graph/api/resources/teams-api-overview#microsoft-teams-limits)和[投票要求](/graph/api/resources/teams-api-overview#polling-requirements)。

### <a name="microsoft-graph-change-notifications-subscription-operations"></a>Microsoft Graph 更改通知订阅操作

以下限制适用于 `/subscriptions` 上的所有请求。

| 操作                 | 每个租户每个应用限制     | 所有租户中的每个应用限制 |
|---------------------------|------------------------------|-----------------------------------|
| POST, PUT, DELETE, PATCH  | 每 20 秒 1000 个请求 | 每 20 秒 2000 个请求      |
| 所有其他 HTTP 方法    | 每 20 秒 5000 个请求 | 每 20 秒 10000 个请求     |
