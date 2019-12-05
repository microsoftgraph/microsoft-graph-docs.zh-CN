---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅“设置用户数据更改的通知”。
localization_priority: Normal
author: piotrci
doc_type: conceptualPageType
ms.prod: ''
ms.openlocfilehash: c951e83348134ee2a5b85e5091377d55a5fd1027
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844244"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="81379-106">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="81379-106">Use the Microsoft Graph API to get change notifications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81379-107">Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="81379-107">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="81379-108">客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="81379-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="81379-109">客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="81379-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="81379-110">有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="81379-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="81379-111">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="81379-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="81379-112">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="81379-112">Outlook [message][]</span></span>
- <span data-ttu-id="81379-113">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="81379-113">Outlook [event][]</span></span>
- <span data-ttu-id="81379-114">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="81379-114">Outlook personal [contact][]</span></span>
- <span data-ttu-id="81379-115">[用户][]</span><span class="sxs-lookup"><span data-stu-id="81379-115">[user][]</span></span>
- <span data-ttu-id="81379-116">[组][]</span><span class="sxs-lookup"><span data-stu-id="81379-116">[group][]</span></span>
- <span data-ttu-id="81379-117">Office 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="81379-117">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="81379-118">用户个人 OneDrive 上_任何_ [driveItem][] 文件夹层次结构内的内容</span><span class="sxs-lookup"><span data-stu-id="81379-118">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="81379-119">OneDrive for Business 上 [driveItem][] _根文件夹_层次结构内的内容</span><span class="sxs-lookup"><span data-stu-id="81379-119">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="81379-120">[chatMessage][]</span><span class="sxs-lookup"><span data-stu-id="81379-120">[chatMessage][]</span></span>
- <span data-ttu-id="81379-121">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="81379-121">Security [alert][]</span></span>

## <a name="permissions"></a><span data-ttu-id="81379-122">权限</span><span class="sxs-lookup"><span data-stu-id="81379-122">Permissions</span></span>

<span data-ttu-id="81379-123">通常订阅操作需要拥有对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="81379-123">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="81379-124">例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="81379-124">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="81379-125">[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。</span><span class="sxs-lookup"><span data-stu-id="81379-125">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="81379-126">下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="81379-126">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="81379-127">权限类型</span><span class="sxs-lookup"><span data-stu-id="81379-127">Permission type</span></span>                        | <span data-ttu-id="81379-128">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="81379-128">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="81379-129">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="81379-129">Delegated - work or school account</span></span>     | <span data-ttu-id="81379-130">[警报][]、[联系人][]、[对话][]、[driveItem][]、[事件][]、[组][]、[邮件][]、[用户][]</span><span class="sxs-lookup"><span data-stu-id="81379-130">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="81379-131">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="81379-131">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="81379-132">[联系人][]、[driveItem][]、[事件][]、[邮件][]</span><span class="sxs-lookup"><span data-stu-id="81379-132">[contact][], [driveItem][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="81379-133">应用程序</span><span class="sxs-lookup"><span data-stu-id="81379-133">Application</span></span>                            | <span data-ttu-id="81379-134">[alert][]、 [contact][]、 [driveItem][]、 [event][]、 [group][]、 [message][]、 [user][]、[了 chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="81379-134">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][], [chatMessage][]</span></span>|

## <a name="see-also"></a><span data-ttu-id="81379-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="81379-135">See also</span></span>

- [<span data-ttu-id="81379-136">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="81379-136">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="81379-137">列出订阅</span><span class="sxs-lookup"><span data-stu-id="81379-137">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="81379-138">获取订阅</span><span class="sxs-lookup"><span data-stu-id="81379-138">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="81379-139">创建订阅</span><span class="sxs-lookup"><span data-stu-id="81379-139">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="81379-140">更新订阅</span><span class="sxs-lookup"><span data-stu-id="81379-140">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="81379-141">删除订阅</span><span class="sxs-lookup"><span data-stu-id="81379-141">Delete subscription</span></span>](../api/subscription-delete.md)

[chatMessage]: ./chatmessage.md
[联系人]: ./contact.md
[contact]: ./contact.md
[对话]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[事件]: ./event.md
[event]: ./event.md
[组]: ./group.md
[group]: ./group.md
[邮件]: ./message.md
[message]: ./message.md
[用户]: ./user.md
[user]: ./user.md
[警报]: ./alert.md
[alert]: ./alert.md
