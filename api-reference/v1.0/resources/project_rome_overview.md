# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="f6322-101">使用 Microsoft Graph API 来处理项目 Rome</span><span class="sxs-lookup"><span data-stu-id="f6322-101">Use the Microsoft Graph API to work with Project Rome</span></span>

<span data-ttu-id="f6322-102">[项目 Rome](https://developer.microsoft.com/en-us/windows/project-rome)是 Microsoft 计划中，以构建一个跨设备体验平台。</span><span class="sxs-lookup"><span data-stu-id="f6322-102">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a cross-device experiences platform.</span></span> <span data-ttu-id="f6322-103">当用户注销，使用客户端设备上登录这些用户使用同一 Microsoft 帐户时，项目 Rome 启用上进行交互的应用程序的本地客户端或服务应用程序和远程主机上的服务。</span><span class="sxs-lookup"><span data-stu-id="f6322-103">Project Rome enables an app on a local client or service to interact with apps and services on a remote host when the user signs in with the same Microsoft account that they use to sign in on the client device.</span></span> <span data-ttu-id="f6322-104">这将允许您围绕用户任务，而不是设备的程序跨设备和跨平台体验。</span><span class="sxs-lookup"><span data-stu-id="f6322-104">This allows you to program cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span>

<span data-ttu-id="f6322-105">通过 Microsoft Graph 启用这些体验公开的关键组件： 活动。</span><span class="sxs-lookup"><span data-stu-id="f6322-105">A key component is exposed via Microsoft Graph to enable these experiences: activities.</span></span>

## <a name="activities"></a><span data-ttu-id="f6322-106">活动</span><span class="sxs-lookup"><span data-stu-id="f6322-106">Activities</span></span>

<span data-ttu-id="f6322-107">跨设备和平台中，Microsoft Graph 中的活动使您能够与您的应用程序的驱动器用户工作效率。</span><span class="sxs-lookup"><span data-stu-id="f6322-107">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="f6322-108">活动用户工作效率的单位，包括三个组件：</span><span class="sxs-lookup"><span data-stu-id="f6322-108">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="f6322-109">深度链接</span><span class="sxs-lookup"><span data-stu-id="f6322-109">A deep link</span></span>
- <span data-ttu-id="f6322-110">直观表示形式</span><span class="sxs-lookup"><span data-stu-id="f6322-110">A visual representation</span></span>
- <span data-ttu-id="f6322-111">描述该活动的内容元数据使用[https://schema.org/](https://schema.org/)共享词汇</span><span class="sxs-lookup"><span data-stu-id="f6322-111">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="f6322-112">应用程序创建会话时, 的历史记录项添加到活动的以反映用户工作效率期。</span><span class="sxs-lookup"><span data-stu-id="f6322-112">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="f6322-113">每次用户 reengages 与活动，新的历史记录项添加到活动以应计用户工作效率。</span><span class="sxs-lookup"><span data-stu-id="f6322-113">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="f6322-114">当应用程序发布用户活动对象时，该对象将显示某些 Windows; 中新的 UI 曲面例如，Cortana 通知和日程表。</span><span class="sxs-lookup"><span data-stu-id="f6322-114">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="f6322-115">活动对象中，可以指定丰富的元数据 （以允许活动在适当的上下文中呈现） 和丰富的视觉效果 （使用[自适应卡片](https://adaptivecards.io/)标记）。</span><span class="sxs-lookup"><span data-stu-id="f6322-115">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="f6322-116">以下 Microsoft Graph Api 可用于创建和检索用户活动：</span><span class="sxs-lookup"><span data-stu-id="f6322-116">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="f6322-117">创建或替换活动</span><span class="sxs-lookup"><span data-stu-id="f6322-117">Create or replace activity</span></span>](../api/projectrome_put_activity.md)
- [<span data-ttu-id="f6322-118">获取活动</span><span class="sxs-lookup"><span data-stu-id="f6322-118">Get activities</span></span>](../api/projectrome_get_activities.md)
- [<span data-ttu-id="f6322-119">获取最近的活动</span><span class="sxs-lookup"><span data-stu-id="f6322-119">Get recent activities</span></span>](../api/projectrome_get_recent_activities.md)
- [<span data-ttu-id="f6322-120">删除活动</span><span class="sxs-lookup"><span data-stu-id="f6322-120">Delete an activity</span></span>](../api/projectrome_delete_activity.md)
- [<span data-ttu-id="f6322-121">创建或替换历史记录项</span><span class="sxs-lookup"><span data-stu-id="f6322-121">Create or replace a history item</span></span>](../api/projectrome_put_historyitem.md)
- [<span data-ttu-id="f6322-122">删除历史记录项</span><span class="sxs-lookup"><span data-stu-id="f6322-122">Delete a history item</span></span>](../api/projectrome_delete_historyitem.md)

