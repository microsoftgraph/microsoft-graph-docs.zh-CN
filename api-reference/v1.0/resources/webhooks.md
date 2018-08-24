# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="e3741-101">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="e3741-101">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="e3741-102">Microsoft Graph REST API 使用 Webhook 机制将通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="e3741-102">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="e3741-103">客户端是一种 Web 服务，用于配置自己的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="e3741-103">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="e3741-104">在发生变更时，客户端应用程序使用通知更新其状态。</span><span class="sxs-lookup"><span data-stu-id="e3741-104">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="e3741-105">有关详细信息，包括如何订阅和处理收到的通知，请参阅 [设置用户数据中更改的通知](../../../concepts/webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="e3741-105">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](../../../concepts/webhooks.md).</span></span>

<span data-ttu-id="e3741-106">使用 Microsoft Graph API，应用程序可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="e3741-106">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="e3741-107">邮件</span><span class="sxs-lookup"><span data-stu-id="e3741-107">Messages</span></span>
- <span data-ttu-id="e3741-108">事件</span><span class="sxs-lookup"><span data-stu-id="e3741-108">Events</span></span>
- <span data-ttu-id="e3741-109">联系人</span><span class="sxs-lookup"><span data-stu-id="e3741-109">Contacts</span></span>
- <span data-ttu-id="e3741-110">用户</span><span class="sxs-lookup"><span data-stu-id="e3741-110">Users</span></span>
- <span data-ttu-id="e3741-111">组</span><span class="sxs-lookup"><span data-stu-id="e3741-111">Groups</span></span>
- <span data-ttu-id="e3741-112">组对话</span><span class="sxs-lookup"><span data-stu-id="e3741-112">Group conversations</span></span>
- <span data-ttu-id="e3741-113">OneDrive 上共享的内容，包括与 SharePoint 网站关联的驱动器</span><span class="sxs-lookup"><span data-stu-id="e3741-113">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="e3741-114">用户的个人 OneDrive 文件夹</span><span class="sxs-lookup"><span data-stu-id="e3741-114">User's personal OneDrive folders</span></span>

## <a name="permissions"></a><span data-ttu-id="e3741-115">权限</span><span class="sxs-lookup"><span data-stu-id="e3741-115">Permissions</span></span>

<span data-ttu-id="e3741-p102">通常订阅操作需要拥有对资源的读取权限。例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。[创建订阅](../api/subscription_post_subscriptions.md)一文列出了各个资源类型所需的权限。下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="e3741-p102">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="e3741-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3741-120">Permission type</span></span>                        | <span data-ttu-id="e3741-121">v1.0 中支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="e3741-121">Supported resource types in v1.0</span></span>                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="e3741-122">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="e3741-122">Delegated - work or school account</span></span>     | <span data-ttu-id="e3741-123">[contact][]、[conversation][]、[drive][]、[event][]、[message][]</span><span class="sxs-lookup"><span data-stu-id="e3741-123">[contact][], [conversation][], [drive][], [event][], [message][]</span></span> |
| <span data-ttu-id="e3741-124">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="e3741-124">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="e3741-125">无</span><span class="sxs-lookup"><span data-stu-id="e3741-125">None</span></span>                                                             |
| <span data-ttu-id="e3741-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3741-126">Application</span></span>                            | <span data-ttu-id="e3741-127">[contact][]、[conversation][]、[event][]、[message][]</span><span class="sxs-lookup"><span data-stu-id="e3741-127">[contact][], [conversation][], [event][], [message][]</span></span>            |

## <a name="see-also"></a><span data-ttu-id="e3741-128">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e3741-128">See also</span></span>

- [<span data-ttu-id="e3741-129">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="e3741-129">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="e3741-130">获取订阅</span><span class="sxs-lookup"><span data-stu-id="e3741-130">Get subscription</span></span>](../api/subscription_get.md)
- [<span data-ttu-id="e3741-131">创建订阅</span><span class="sxs-lookup"><span data-stu-id="e3741-131">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
- [<span data-ttu-id="e3741-132">更新订阅</span><span class="sxs-lookup"><span data-stu-id="e3741-132">Update subscription</span></span>](../api/subscription_update.md)
- [<span data-ttu-id="e3741-133">删除订阅</span><span class="sxs-lookup"><span data-stu-id="e3741-133">Delete subscription</span></span>](../api/subscription_delete.md)

[联系人]: ./contact.md
[contact]: ./contact.md
[对话]: ./conversation.md
[conversation]: ./conversation.md
[驱动器]: ./drive.md
[drive]: ./drive.md
[事件]: ./event.md
[event]: ./event.md
[邮件]: ./message.md
[message]: ./message.md
