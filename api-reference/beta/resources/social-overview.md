---
title: 使用 Microsoft Graph API 在应用中集成人员和工作区智能
description: Microsoft Graph 允许访问相关人员的有用数据、其个人资料、与之交互的文档和工作模式，并支持用户社交环境中的手势。
localization_priority: Priority
author: simonhult
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 9085db75d70932fe3364b5739a33fc480f30032a
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844258"
---
# <a name="use-the-microsoft-graph-api-to-integrate-people-and-workplace-intelligence-in-an-app"></a><span data-ttu-id="38c46-103">使用 Microsoft Graph API 在应用中集成人员和工作区智能</span><span class="sxs-lookup"><span data-stu-id="38c46-103">Use the Microsoft Graph API to integrate people and workplace intelligence in an app</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38c46-104">Microsoft Graph 允许访问相关人员的有用数据、其个人资料、与之交互的文档和工作模式，并支持用户社交环境中的手势。</span><span class="sxs-lookup"><span data-stu-id="38c46-104">Microsoft Graph enables access to useful data about people, their profile, documents they interact with, and work patterns, and supports gestures in a user's social context.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="38c46-105">聚合并提取有关人员的特定信息</span><span class="sxs-lookup"><span data-stu-id="38c46-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="38c46-106">功能：人员</span><span class="sxs-lookup"><span data-stu-id="38c46-106">Feature: People</span></span>

<span data-ttu-id="38c46-107">你可以使用 [person](../resources/person.md) 资源和 People API 从邮件、联系人和社交网络中聚合某个人员的相关信息。</span><span class="sxs-lookup"><span data-stu-id="38c46-107">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="38c46-108">根据多种通信、协作和业务关系按相关性对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="38c46-108">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="38c46-109">通过此 API 可以基于自己的条件对人员进行浏览、排序、选择、筛选或搜索。</span><span class="sxs-lookup"><span data-stu-id="38c46-109">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="38c46-110">列出人员</span><span class="sxs-lookup"><span data-stu-id="38c46-110">List people</span></span>](../api/user-list-people.md)

## <a name="help-users-contextualize-others-in-their-organization"></a><span data-ttu-id="38c46-111">帮助用户将组织内的其他用户置于上下文中考虑</span><span class="sxs-lookup"><span data-stu-id="38c46-111">Help users contextualize others in their organization</span></span>

<span data-ttu-id="38c46-112">功能：个人资料（预览版）</span><span class="sxs-lookup"><span data-stu-id="38c46-112">Feature: Profile (preview)</span></span>

<span data-ttu-id="38c46-113">若要将组织内的其他人员置于上下文中考虑，通常会查看人员的个人资料或个人资料卡片。</span><span class="sxs-lookup"><span data-stu-id="38c46-113">People who seek to contextualize others within their organization commonly view a person's profile or profile card.</span></span> 

<span data-ttu-id="38c46-114">[profile](../resources/profile.md) 资源是关于租户内人员的信息的丰富源，提供了用于存储和检索人员信息的轻型机制。</span><span class="sxs-lookup"><span data-stu-id="38c46-114">The [profile](../resources/profile.md) resource is a rich source of information about people within a tenant and provides a lightweight mechanism for storing and retrieving information about a person.</span></span> 

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a><span data-ttu-id="38c46-115">帮助用户获得最相关的工作文档</span><span class="sxs-lookup"><span data-stu-id="38c46-115">Help users get the most relevant documents for their work</span></span>

<span data-ttu-id="38c46-116">功能：文档见解</span><span class="sxs-lookup"><span data-stu-id="38c46-116">Feature: Document insights</span></span>

<span data-ttu-id="38c46-117">使用见解 API 为用户标识最相关的文档：</span><span class="sxs-lookup"><span data-stu-id="38c46-117">Use the insights API to identify the most relevant documents for a user:</span></span>

- <span data-ttu-id="38c46-118">列出用户[常用的](../api/insights-list-trending.md)文档</span><span class="sxs-lookup"><span data-stu-id="38c46-118">List documents [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="38c46-119">列出用户[使用的](../api/insights-list-used.md)文档</span><span class="sxs-lookup"><span data-stu-id="38c46-119">List documents [used by](../api/insights-list-used.md) a user</span></span>
- <span data-ttu-id="38c46-120">列出[与用户共享或由用户共享的](../api/insights-list-shared.md)文档</span><span class="sxs-lookup"><span data-stu-id="38c46-120">List documents [shared with or shared by](../api/insights-list-shared.md) a user</span></span>

## <a name="manage--mentions"></a><span data-ttu-id="38c46-121">管理 @提及</span><span class="sxs-lookup"><span data-stu-id="38c46-121">Manage @-Mentions</span></span>

<span data-ttu-id="38c46-122">功能：@-提及（预览版）</span><span class="sxs-lookup"><span data-stu-id="38c46-122">Feature: @-mentions (preview)</span></span>

<span data-ttu-id="38c46-123">标注要通知的收件人并在邮件中引起该收件人的注意是一种常见的社交手势。</span><span class="sxs-lookup"><span data-stu-id="38c46-123">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="38c46-124">[mention](../resources/mention.md) 资源和 Mentions API 提供了一种轻型机制，可以在[邮件](../resources/message.md)中标注收件人，获取使用 @提及功能向用户发出通知的所有邮件，或者获取邮件中的每个提及。</span><span class="sxs-lookup"><span data-stu-id="38c46-124">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="38c46-125">在新邮件中创建提及</span><span class="sxs-lookup"><span data-stu-id="38c46-125">Create mentions in a new message</span></span>

  - [<span data-ttu-id="38c46-126">将提及作为新邮件的一部分进行创建并发送</span><span class="sxs-lookup"><span data-stu-id="38c46-126">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="38c46-127">将提及作为邮件草稿的一部分进行创建</span><span class="sxs-lookup"><span data-stu-id="38c46-127">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="38c46-128">获取有关邮件中的提及的信息</span><span class="sxs-lookup"><span data-stu-id="38c46-128">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="38c46-129">获取已登录用户的邮箱中提及该用户的所有邮件</span><span class="sxs-lookup"><span data-stu-id="38c46-129">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="38c46-130">获取邮件中的每个提及的详细信息</span><span class="sxs-lookup"><span data-stu-id="38c46-130">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="38c46-131">[删除邮件中的提及](../api/message-delete.md#request-2)</span><span class="sxs-lookup"><span data-stu-id="38c46-131">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>


## <a name="help-users-gain-insights-into-their-work-patterns"></a><span data-ttu-id="38c46-132">帮助用户深入了解其工作模式</span><span class="sxs-lookup"><span data-stu-id="38c46-132">Help users gain insights into their work patterns</span></span>

<span data-ttu-id="38c46-133">功能：分析（预览版）</span><span class="sxs-lookup"><span data-stu-id="38c46-133">Feature: Analytics (preview)</span></span>

<span data-ttu-id="38c46-134">使用分析 API 获取用户的活动统计信息及相关设置：</span><span class="sxs-lookup"><span data-stu-id="38c46-134">Use the analytics API to get activity statistics and related settings for a user:</span></span>

- <span data-ttu-id="38c46-135">[设置](../resources/settings.md)：要让分析 API 为用户返回结果，当前用户分析设置必须显示有效的 MyAnalytics 许可证、选择使用 MyAnalytics，并具有启用了图形的云托管邮箱。</span><span class="sxs-lookup"><span data-stu-id="38c46-135">[settings](../resources/settings.md): For the analytics API to return results for a user, the current user analytics settings must show a valid MyAnalytics license, be opted in to using MyAnalytics, and have a cloud-hosted mailbox that’s graph-enabled.</span></span>
- <span data-ttu-id="38c46-136">[activityStatistics](../resources/activitystatistics.md)：获取整个上周用户花时间参与的 Office 365 活动的相关数据，包括工作时间内及工作之余在[通话](callactivitystatistics.md)、[聊天（即时消息）](chatactivitystatistics.md)、[电子邮件](emailactivitystatistics.md)和[会议](meetingactivitystatistics.md)上花费的小时数，以及可用于[专注工作](focusactivitystatistics.md)的小时数。</span><span class="sxs-lookup"><span data-stu-id="38c46-136">[activityStatistics](../resources/activitystatistics.md): Gets data for the last complete week (or the specified time range) for the Office 365 activities that a user spent time on, including the number of hours spent on [calls](callactivitystatistics.md), [chats (instant messages)](chatactivitystatistics.md), [email](emailactivitystatistics.md), and [meetings](meetingactivitystatistics.md) during and outside of working hours and the number of hours available for [focused work](focusactivitystatistics.md).</span></span>
