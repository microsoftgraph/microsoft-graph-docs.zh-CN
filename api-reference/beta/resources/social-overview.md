---
title: 使用 Microsoft Graph API 在应用程序中集成社交智能
description: Microsoft Graph 支持用户社交环境中的社交手势，并提供对有用人员和社交数据的访问权限。
localization_priority: Priority
author: simonhult
ms.prod: insights
ms.openlocfilehash: 45482d2e47c97b6c09302ab60ff9c031cef1e92a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345683"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a><span data-ttu-id="9363e-103">使用 Microsoft Graph API 在应用程序中集成社交智能</span><span class="sxs-lookup"><span data-stu-id="9363e-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9363e-104">Microsoft Graph 支持用户社交环境中的社交手势，并提供对有用人员和社交数据的访问权限。</span><span class="sxs-lookup"><span data-stu-id="9363e-104">Microsoft Graph supports social gestures in a user's social context, and provides access to useful people and social data.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="9363e-105">聚合并提取有关人员的特定信息</span><span class="sxs-lookup"><span data-stu-id="9363e-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="9363e-106">你可以使用 [person](../resources/person.md) 资源和 People API 从邮件、联系人和社交网络中聚合某个人员的相关信息。</span><span class="sxs-lookup"><span data-stu-id="9363e-106">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="9363e-107">根据多种通信、协作和业务关系按相关性对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="9363e-107">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="9363e-108">通过此 API 可以基于自己的条件对人员进行浏览、排序、选择、筛选或搜索。</span><span class="sxs-lookup"><span data-stu-id="9363e-108">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="9363e-109">列出人员</span><span class="sxs-lookup"><span data-stu-id="9363e-109">List people</span></span>](../api/user-list-people.md)

## <a name="manage--mentions"></a><span data-ttu-id="9363e-110">管理 @提及</span><span class="sxs-lookup"><span data-stu-id="9363e-110">Manage @-Mentions</span></span>

<span data-ttu-id="9363e-111">标注要通知的收件人并在邮件中引起该收件人的注意是一种常见的社交手势。</span><span class="sxs-lookup"><span data-stu-id="9363e-111">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="9363e-112">[mention](../resources/mention.md) 资源和 Mentions API 提供了一种轻型机制，可以在[邮件](../resources/message.md)中标注收件人，获取使用 @提及功能向用户发出通知的所有邮件，或者获取邮件中的每个提及。</span><span class="sxs-lookup"><span data-stu-id="9363e-112">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="9363e-113">在新邮件中创建提及</span><span class="sxs-lookup"><span data-stu-id="9363e-113">Create mentions in a new message</span></span>

  - [<span data-ttu-id="9363e-114">将提及作为新邮件的一部分进行创建并发送</span><span class="sxs-lookup"><span data-stu-id="9363e-114">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="9363e-115">将提及作为邮件草稿的一部分进行创建</span><span class="sxs-lookup"><span data-stu-id="9363e-115">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="9363e-116">获取有关邮件中的提及的信息</span><span class="sxs-lookup"><span data-stu-id="9363e-116">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="9363e-117">获取已登录用户的邮箱中提及该用户的所有邮件</span><span class="sxs-lookup"><span data-stu-id="9363e-117">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="9363e-118">获取邮件中的每个提及的详细信息</span><span class="sxs-lookup"><span data-stu-id="9363e-118">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="9363e-119">[删除邮件中的提及](../api/message-delete.md#request-2)</span><span class="sxs-lookup"><span data-stu-id="9363e-119">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>

## <a name="access-social-data-around-and-about-a-user"></a><span data-ttu-id="9363e-120">访问有关用户的社交数据</span><span class="sxs-lookup"><span data-stu-id="9363e-120">Access social data around and about a user</span></span>

<span data-ttu-id="9363e-121">Office Graph 封装了 Office 365 中的不同实体之间的关系。</span><span class="sxs-lookup"><span data-stu-id="9363e-121">Office Graph encapsulates the relationships between different entities in Office 365.</span></span> <span data-ttu-id="9363e-122">使用 Office Graph 获取 Office 365 中的各个用户的社交见解。</span><span class="sxs-lookup"><span data-stu-id="9363e-122">Use Office Graph to get social insights into individual users across Office 365.</span></span>

- <span data-ttu-id="9363e-123">列出用户[常用的项目](../api/insights-list-trending.md)</span><span class="sxs-lookup"><span data-stu-id="9363e-123">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="9363e-124">列出与某个用户[合作](../api/user-list-people.md)的用户</span><span class="sxs-lookup"><span data-stu-id="9363e-124">List users who have been [working with](../api/user-list-people.md) a user</span></span>
