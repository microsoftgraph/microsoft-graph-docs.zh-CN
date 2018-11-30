---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 webhook 机制来将通知传递到客户端。 客户端是配置其自己的 URL，以接收通知的 web 服务。 客户端应用程序使用通知更新时更改其状态。 有关详细信息，包括如何订阅和处理传入通知，请参阅 Set up 中用户数据的更改的通知。
ms.openlocfilehash: a44a32b5a1dd1c8f3bd2a9234503da5a583f8bdd
ms.sourcegitcommit: 2532b8dd7f2533d956e2600855b3daeabdd9b8ff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2018
ms.locfileid: "27011767"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="e2e2d-106">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="e2e2d-106">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="e2e2d-107">Microsoft Graph REST API 使用 webhook 机制来将通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="e2e2d-107">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="e2e2d-108">客户端是配置其自己的 URL，以接收通知的 web 服务。</span><span class="sxs-lookup"><span data-stu-id="e2e2d-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="e2e2d-109">客户端应用程序使用通知更新时更改其状态。</span><span class="sxs-lookup"><span data-stu-id="e2e2d-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="e2e2d-110">有关详细信息，包括如何订阅和处理传入通知，请参阅[设置通知用户数据中的更改](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="e2e2d-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="e2e2d-111">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="e2e2d-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="e2e2d-112">邮件</span><span class="sxs-lookup"><span data-stu-id="e2e2d-112">Messages</span></span>
- <span data-ttu-id="e2e2d-113">事件</span><span class="sxs-lookup"><span data-stu-id="e2e2d-113">Events</span></span>
- <span data-ttu-id="e2e2d-114">联系人</span><span class="sxs-lookup"><span data-stu-id="e2e2d-114">Contacts</span></span>
- <span data-ttu-id="e2e2d-115">用户</span><span class="sxs-lookup"><span data-stu-id="e2e2d-115">Users</span></span>
- <span data-ttu-id="e2e2d-116">组</span><span class="sxs-lookup"><span data-stu-id="e2e2d-116">Groups</span></span>
- <span data-ttu-id="e2e2d-117">组对话</span><span class="sxs-lookup"><span data-stu-id="e2e2d-117">Group conversations</span></span>
- <span data-ttu-id="e2e2d-118">在 OneDrive，包括与 SharePoint 网站关联的驱动器上共享的内容</span><span class="sxs-lookup"><span data-stu-id="e2e2d-118">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="e2e2d-119">用户的个人 OneDrive 文件夹</span><span class="sxs-lookup"><span data-stu-id="e2e2d-119">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="e2e2d-120">安全警报</span><span class="sxs-lookup"><span data-stu-id="e2e2d-120">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="e2e2d-121">Permissions</span><span class="sxs-lookup"><span data-stu-id="e2e2d-121">Permissions</span></span>

<span data-ttu-id="e2e2d-p103">通常订阅操作需要拥有对资源的读取权限。例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="e2e2d-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="e2e2d-126">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2e2d-126">Permission type</span></span>                        | <span data-ttu-id="e2e2d-127">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="e2e2d-127">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="e2e2d-128">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="e2e2d-128">Delegated - work or school account</span></span>     | <span data-ttu-id="e2e2d-129">[联系人][]、[对话][]、[驱动器][]、[事件][]、[组][]、[消息][]、[用户][]、[通知][]</span><span class="sxs-lookup"><span data-stu-id="e2e2d-129">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |
| <span data-ttu-id="e2e2d-130">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="e2e2d-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="e2e2d-131">[联系人][]、[驱动器][]、[事件][]、[消息][]</span><span class="sxs-lookup"><span data-stu-id="e2e2d-131">[contact][], [drive][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="e2e2d-132">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2e2d-132">Application</span></span>                            | <span data-ttu-id="e2e2d-133">[联系人][]、[对话][]、[驱动器][]、[事件][]、[组][]、[消息][]、[用户][]、[通知][]</span><span class="sxs-lookup"><span data-stu-id="e2e2d-133">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="e2e2d-134">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e2e2d-134">See also</span></span>

- [<span data-ttu-id="e2e2d-135">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="e2e2d-135">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="e2e2d-136">获取订阅</span><span class="sxs-lookup"><span data-stu-id="e2e2d-136">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="e2e2d-137">创建订阅</span><span class="sxs-lookup"><span data-stu-id="e2e2d-137">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="e2e2d-138">更新订阅</span><span class="sxs-lookup"><span data-stu-id="e2e2d-138">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="e2e2d-139">删除订阅</span><span class="sxs-lookup"><span data-stu-id="e2e2d-139">Delete subscription</span></span>](../api/subscription-delete.md)

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