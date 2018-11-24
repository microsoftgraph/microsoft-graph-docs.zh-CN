# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="efcf8-101">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="efcf8-101">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="efcf8-102">Microsoft Graph REST API 使用 webhook 机制来将通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="efcf8-102">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="efcf8-103">客户端是配置其自己的 URL，以接收通知的 web 服务。</span><span class="sxs-lookup"><span data-stu-id="efcf8-103">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="efcf8-104">客户端应用程序使用通知更新时更改其状态。</span><span class="sxs-lookup"><span data-stu-id="efcf8-104">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="efcf8-105">有关详细信息，包括如何订阅和处理传入通知，请参阅[设置通知用户数据中的更改](../../../concepts/webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="efcf8-105">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](../../../concepts/webhooks.md).</span></span>

<span data-ttu-id="efcf8-106">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="efcf8-106">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="efcf8-107">邮件</span><span class="sxs-lookup"><span data-stu-id="efcf8-107">Messages</span></span>
- <span data-ttu-id="efcf8-108">事件</span><span class="sxs-lookup"><span data-stu-id="efcf8-108">Events</span></span>
- <span data-ttu-id="efcf8-109">联系人</span><span class="sxs-lookup"><span data-stu-id="efcf8-109">Contacts</span></span>
- <span data-ttu-id="efcf8-110">用户</span><span class="sxs-lookup"><span data-stu-id="efcf8-110">Users</span></span>
- <span data-ttu-id="efcf8-111">组</span><span class="sxs-lookup"><span data-stu-id="efcf8-111">Groups</span></span>
- <span data-ttu-id="efcf8-112">组对话</span><span class="sxs-lookup"><span data-stu-id="efcf8-112">Group conversations</span></span>
- <span data-ttu-id="efcf8-113">在 OneDrive，包括与 SharePoint 网站关联的驱动器上共享的内容</span><span class="sxs-lookup"><span data-stu-id="efcf8-113">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="efcf8-114">用户的个人 OneDrive 文件夹</span><span class="sxs-lookup"><span data-stu-id="efcf8-114">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="efcf8-115">安全警报</span><span class="sxs-lookup"><span data-stu-id="efcf8-115">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="efcf8-116">Permissions</span><span class="sxs-lookup"><span data-stu-id="efcf8-116">Permissions</span></span>

<span data-ttu-id="efcf8-p102">通常订阅操作需要拥有对资源的读取权限。例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。[创建订阅](../api/subscription_post_subscriptions.md)一文列出了各个资源类型所需的权限。下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="efcf8-p102">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="efcf8-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="efcf8-121">Permission type</span></span>                        | <span data-ttu-id="efcf8-122">v1.0 中支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="efcf8-122">Supported resource types in v1.0</span></span>                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="efcf8-123">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="efcf8-123">Delegated - work or school account</span></span>     | <span data-ttu-id="efcf8-124">[联系人][]、[对话][]、[驱动器][]、[事件][]、[邮件][]、[通知][]</span><span class="sxs-lookup"><span data-stu-id="efcf8-124">[contact][], [conversation][], [drive][], [event][], [message][], [alert][]</span></span> |
| <span data-ttu-id="efcf8-125">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="efcf8-125">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="efcf8-126">无</span><span class="sxs-lookup"><span data-stu-id="efcf8-126">None</span></span>                                                             |
| <span data-ttu-id="efcf8-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="efcf8-127">Application</span></span>                            | <span data-ttu-id="efcf8-128">[联系人][]、[对话][]、[事件][]、[消息][]、[警报][]</span><span class="sxs-lookup"><span data-stu-id="efcf8-128">[contact][], [conversation][], [event][], [message][], [alert][]</span></span>           |

## <a name="see-also"></a><span data-ttu-id="efcf8-129">另请参阅</span><span class="sxs-lookup"><span data-stu-id="efcf8-129">See also</span></span>

- [<span data-ttu-id="efcf8-130">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="efcf8-130">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="efcf8-131">获取订阅</span><span class="sxs-lookup"><span data-stu-id="efcf8-131">Get subscription</span></span>](../api/subscription_get.md)
- [<span data-ttu-id="efcf8-132">创建订阅</span><span class="sxs-lookup"><span data-stu-id="efcf8-132">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
- [<span data-ttu-id="efcf8-133">更新订阅</span><span class="sxs-lookup"><span data-stu-id="efcf8-133">Update subscription</span></span>](../api/subscription_update.md)
- [<span data-ttu-id="efcf8-134">删除订阅</span><span class="sxs-lookup"><span data-stu-id="efcf8-134">Delete subscription</span></span>](../api/subscription_delete.md)

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
[通知]: ./alert.md
[alert]: ./alert.md