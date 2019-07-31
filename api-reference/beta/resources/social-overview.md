---
title: 使用 Microsoft Graph API 在应用中集成社交和工作区智能
description: Microsoft Graph 支持用户社交环境中的社交手势，并提供对有用人员和社交数据的访问权限。
localization_priority: Priority
author: simonhult
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 84e0c82173dad6f08d5911f32ef5c384f041ea19
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008087"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-and-workplace-intelligence-in-an-app"></a><span data-ttu-id="0d0e4-103">使用 Microsoft Graph API 在应用中集成社交和工作区智能</span><span class="sxs-lookup"><span data-stu-id="0d0e4-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d0e4-104">Microsoft Graph 支持用户社交环境中的社交手势，并提供对有用人员和社交数据的访问权限。</span><span class="sxs-lookup"><span data-stu-id="0d0e4-104">Microsoft Graph supports social gestures in a user's social context, and provides access to useful people and social data.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="0d0e4-105">聚合并提取有关人员的特定信息</span><span class="sxs-lookup"><span data-stu-id="0d0e4-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="0d0e4-106">你可以使用 [person](../resources/person.md) 资源和 People API 从邮件、联系人和社交网络中聚合某个人员的相关信息。</span><span class="sxs-lookup"><span data-stu-id="0d0e4-106">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="0d0e4-107">根据多种通信、协作和业务关系按相关性对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="0d0e4-107">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="0d0e4-108">通过此 API 可以基于自己的条件对人员进行浏览、排序、选择、筛选或搜索。</span><span class="sxs-lookup"><span data-stu-id="0d0e4-108">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="0d0e4-109">列出人员</span><span class="sxs-lookup"><span data-stu-id="0d0e4-109">List people</span></span>](../api/user-list-people.md)

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a><span data-ttu-id="0d0e4-110">帮助用户获得最相关的工作文档</span><span class="sxs-lookup"><span data-stu-id="0d0e4-110">Help users get the most relevant documents for their work</span></span>

<span data-ttu-id="0d0e4-111">使用见解 API 为用户标识最相关的文档：</span><span class="sxs-lookup"><span data-stu-id="0d0e4-111">Use the insights API to identify the most relevant documents for a user:</span></span> 

- <span data-ttu-id="0d0e4-112">列出用户[常用的](../api/insights-list-trending.md)文档</span><span class="sxs-lookup"><span data-stu-id="0d0e4-112">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="0d0e4-113">列出用户[使用的](../api/insights-list-used.md)文档</span><span class="sxs-lookup"><span data-stu-id="0d0e4-113">List documents [used by](../api/insights-list-used.md) a user</span></span>
- <span data-ttu-id="0d0e4-114">列出[与用户共享或由用户共享的](../api/insights-list-shared.md)文档</span><span class="sxs-lookup"><span data-stu-id="0d0e4-114">List documents [shared with or shared by](../api/insights-list-shared.md) a user</span></span>

## <a name="manage--mentions"></a><span data-ttu-id="0d0e4-115">管理 @提及</span><span class="sxs-lookup"><span data-stu-id="0d0e4-115">Manage @-Mentions</span></span>

<span data-ttu-id="0d0e4-116">标注要通知的收件人并在邮件中引起该收件人的注意是一种常见的社交手势。</span><span class="sxs-lookup"><span data-stu-id="0d0e4-116">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="0d0e4-117">[mention](../resources/mention.md) 资源和 Mentions API 提供了一种轻型机制，可以在[邮件](../resources/message.md)中标注收件人，获取使用 @提及功能向用户发出通知的所有邮件，或者获取邮件中的每个提及。</span><span class="sxs-lookup"><span data-stu-id="0d0e4-117">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="0d0e4-118">在新邮件中创建提及</span><span class="sxs-lookup"><span data-stu-id="0d0e4-118">Create mentions in a new message</span></span>

  - [<span data-ttu-id="0d0e4-119">将提及作为新邮件的一部分进行创建并发送</span><span class="sxs-lookup"><span data-stu-id="0d0e4-119">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="0d0e4-120">将提及作为邮件草稿的一部分进行创建</span><span class="sxs-lookup"><span data-stu-id="0d0e4-120">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="0d0e4-121">获取有关邮件中的提及的信息</span><span class="sxs-lookup"><span data-stu-id="0d0e4-121">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="0d0e4-122">获取已登录用户的邮箱中提及该用户的所有邮件</span><span class="sxs-lookup"><span data-stu-id="0d0e4-122">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="0d0e4-123">获取邮件中的每个提及的详细信息</span><span class="sxs-lookup"><span data-stu-id="0d0e4-123">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="0d0e4-124">[删除邮件中的提及](../api/message-delete.md#request-2)</span><span class="sxs-lookup"><span data-stu-id="0d0e4-124">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>

