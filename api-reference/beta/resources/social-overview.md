---
title: 使用 Microsoft Graph API 将应用程序中的社交智能集成
description: Microsoft Graph 社交手势支持在用户的社交上下文中，并提供对有用的个人和社会数据访问。
localization_priority: Priority
ms.openlocfilehash: b3b71cf1bad0d860978c75c88f0b77a32eab1a0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862487"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a><span data-ttu-id="56ab1-103">使用 Microsoft Graph API 将应用程序中的社交智能集成</span><span class="sxs-lookup"><span data-stu-id="56ab1-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

> <span data-ttu-id="56ab1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="56ab1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56ab1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="56ab1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56ab1-106">Microsoft Graph 社交手势支持在用户的社交上下文中，并提供对有用的个人和社会数据访问。</span><span class="sxs-lookup"><span data-stu-id="56ab1-106">Microsoft Graph supports social gestures in a user's social context, and provides access to useful people and social data.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="56ab1-107">聚合和提取人员相关的特定信息</span><span class="sxs-lookup"><span data-stu-id="56ab1-107">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="56ab1-108">使用邮件、 联系人和社交网络之间的[人员](../resources/person.md)资源和此人的聚合信息的人员 API。</span><span class="sxs-lookup"><span data-stu-id="56ab1-108">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="56ab1-109">按其相关性基于多个通信、 协作和业务关系，对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="56ab1-109">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="56ab1-110">API 可以浏览、 排序、 选择、 筛选器或按条件的人员搜索。</span><span class="sxs-lookup"><span data-stu-id="56ab1-110">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="56ab1-111">List people</span><span class="sxs-lookup"><span data-stu-id="56ab1-111">List people</span></span>](../api/user-list-people.md)

## <a name="manage--mentions"></a><span data-ttu-id="56ab1-112">管理 @ 提及</span><span class="sxs-lookup"><span data-stu-id="56ab1-112">Manage @-Mentions</span></span>

<span data-ttu-id="56ab1-113">调用出收件人通知和消息中获取收件人的注意是常见的社交笔势。</span><span class="sxs-lookup"><span data-stu-id="56ab1-113">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="56ab1-114">[提及](../resources/mention.md)资源和提到 API 提供细线的机制来呼叫出中[邮件](../resources/message.md)的收件人，获取在其中使用 @-提及，通知用户的所有邮件，或都获取一条消息中的每个提及。</span><span class="sxs-lookup"><span data-stu-id="56ab1-114">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="56ab1-115">创建新邮件中提及</span><span class="sxs-lookup"><span data-stu-id="56ab1-115">Create mentions in a new message</span></span>

  - [<span data-ttu-id="56ab1-116">创建和发送提及作为新邮件的一部分</span><span class="sxs-lookup"><span data-stu-id="56ab1-116">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="56ab1-117">创建提及的邮件草稿一部分</span><span class="sxs-lookup"><span data-stu-id="56ab1-117">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="56ab1-118">在邮件中获取提及相关信息</span><span class="sxs-lookup"><span data-stu-id="56ab1-118">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="56ab1-119">获取提及用户的登录用户邮箱中的所有邮件</span><span class="sxs-lookup"><span data-stu-id="56ab1-119">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="56ab1-120">获取一条消息中的每个提及的详细信息</span><span class="sxs-lookup"><span data-stu-id="56ab1-120">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="56ab1-121">在邮件中[删除某个提及](../api/message-delete.md#request-2)</span><span class="sxs-lookup"><span data-stu-id="56ab1-121">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>

## <a name="access-social-data-around-and-about-a-user"></a><span data-ttu-id="56ab1-122">围绕用户以及访问社交数据</span><span class="sxs-lookup"><span data-stu-id="56ab1-122">Access social data around and about a user</span></span>

<span data-ttu-id="56ab1-123">Office 图形封装在 Office 365 中的不同实体之间的关系。</span><span class="sxs-lookup"><span data-stu-id="56ab1-123">Office Graph encapsulates the relationships between different entities in Office 365.</span></span> <span data-ttu-id="56ab1-124">使用 Office 图形跨 Office 365 中获取单个用户的社交见解。</span><span class="sxs-lookup"><span data-stu-id="56ab1-124">Use Office Graph to get social insights into individual users across Office 365.</span></span>

- <span data-ttu-id="56ab1-125">列表项[趋势围绕](../api/insights-list-trending.md)用户</span><span class="sxs-lookup"><span data-stu-id="56ab1-125">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="56ab1-126">列出用户的已[处理](../api/user-list-people.md)的用户</span><span class="sxs-lookup"><span data-stu-id="56ab1-126">List users who have been [working with](../api/user-list-people.md) a user</span></span>
