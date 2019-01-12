---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 webhook 机制来将通知传递到客户端。 客户端是配置其自己的 URL，以接收通知的 web 服务。 客户端应用程序使用通知更新时更改其状态。 有关详细信息，包括如何订阅和处理传入通知，请参阅 Set up 中用户数据的更改的通知。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: fe571fe0a9a7c982ee7ce93b08457586134d7d91
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986132"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="d8a82-106">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="d8a82-106">Use the Microsoft Graph API to get change notifications</span></span>

> <span data-ttu-id="d8a82-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d8a82-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8a82-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d8a82-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8a82-109">Microsoft Graph REST API 使用 webhook 机制来将通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="d8a82-109">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="d8a82-110">客户端是配置其自己的 URL，以接收通知的 web 服务。</span><span class="sxs-lookup"><span data-stu-id="d8a82-110">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="d8a82-111">客户端应用程序使用通知更新时更改其状态。</span><span class="sxs-lookup"><span data-stu-id="d8a82-111">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="d8a82-112">有关详细信息，包括如何订阅和处理传入通知，请参阅[设置通知用户数据中的更改](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="d8a82-112">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="d8a82-113">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="d8a82-113">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="d8a82-114">邮件</span><span class="sxs-lookup"><span data-stu-id="d8a82-114">Messages</span></span>
- <span data-ttu-id="d8a82-115">事件</span><span class="sxs-lookup"><span data-stu-id="d8a82-115">Events</span></span>
- <span data-ttu-id="d8a82-116">联系人</span><span class="sxs-lookup"><span data-stu-id="d8a82-116">Contacts</span></span>
- <span data-ttu-id="d8a82-117">用户</span><span class="sxs-lookup"><span data-stu-id="d8a82-117">Users</span></span>
- <span data-ttu-id="d8a82-118">组</span><span class="sxs-lookup"><span data-stu-id="d8a82-118">Groups</span></span>
- <span data-ttu-id="d8a82-119">组对话</span><span class="sxs-lookup"><span data-stu-id="d8a82-119">Group conversations</span></span>
- <span data-ttu-id="d8a82-120">在 OneDrive，包括与 SharePoint 网站关联的驱动器上共享的内容</span><span class="sxs-lookup"><span data-stu-id="d8a82-120">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="d8a82-121">用户的个人 OneDrive 文件夹</span><span class="sxs-lookup"><span data-stu-id="d8a82-121">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="d8a82-122">安全警报</span><span class="sxs-lookup"><span data-stu-id="d8a82-122">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="d8a82-123">Permissions</span><span class="sxs-lookup"><span data-stu-id="d8a82-123">Permissions</span></span>

<span data-ttu-id="d8a82-p104">通常订阅操作需要拥有对资源的读取权限。例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="d8a82-p104">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="d8a82-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8a82-128">Permission type</span></span>                        | <span data-ttu-id="d8a82-129">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="d8a82-129">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="d8a82-130">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="d8a82-130">Delegated - work or school account</span></span>     | <span data-ttu-id="d8a82-131">[联系人][]、[对话][]、[驱动器][]、[事件][]、[组][]、[消息][]、[用户][]、[通知][]</span><span class="sxs-lookup"><span data-stu-id="d8a82-131">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |
| <span data-ttu-id="d8a82-132">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="d8a82-132">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="d8a82-133">[联系人][]、[驱动器][]、[事件][]、[消息][]</span><span class="sxs-lookup"><span data-stu-id="d8a82-133">[contact][], [drive][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="d8a82-134">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8a82-134">Application</span></span>                            | <span data-ttu-id="d8a82-135">[联系人][]、[对话][]、[驱动器][]、[事件][]、[组][]、[消息][]、[用户][]、[通知][]</span><span class="sxs-lookup"><span data-stu-id="d8a82-135">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="d8a82-136">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d8a82-136">See also</span></span>

- [<span data-ttu-id="d8a82-137">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="d8a82-137">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="d8a82-138">列表订阅</span><span class="sxs-lookup"><span data-stu-id="d8a82-138">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="d8a82-139">获取订阅</span><span class="sxs-lookup"><span data-stu-id="d8a82-139">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="d8a82-140">创建订阅</span><span class="sxs-lookup"><span data-stu-id="d8a82-140">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="d8a82-141">更新订阅</span><span class="sxs-lookup"><span data-stu-id="d8a82-141">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="d8a82-142">删除订阅</span><span class="sxs-lookup"><span data-stu-id="d8a82-142">Delete subscription</span></span>](../api/subscription-delete.md)

[联系人]: ./contact.md
[contact]: ./contact.md
[对话]: ./conversation.md
[conversation]: ./conversation.md
[驱动器]: ./drive.md
[drive]: ./drive.md
[事件]: ./event.md
[event]: ./event.md
[组]: ./group.md
[group]: ./group.md
[邮件]: ./message.md
[message]: ./message.md
[用户]: ./user.md
[user]: ./user.md
[通知]: ./alert.md
[alert]: ./alert.md
