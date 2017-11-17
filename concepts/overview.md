# <a name="overview-of-microsoft-graph"></a><span data-ttu-id="ca64a-101">Microsoft Graph 概述</span><span class="sxs-lookup"><span data-stu-id="ca64a-101">Overview of Microsoft Graph</span></span>

<span data-ttu-id="ca64a-p101">可以使用 Microsoft Graph API 在 Microsoft 云中与数百万用户的数据交互。使用 Microsoft Graph 为组织和消费者生成应用，此类应用与所有这些资源、关系以及情报通过单个终结点相连接：`https://graph.microsoft.com`。</span><span class="sxs-lookup"><span data-stu-id="ca64a-p101">You can use the Microsoft Graph API to interact with the data of millions of users in the Microsoft cloud. Use Microsoft Graph to build apps for organizations and consumers that connect to a wealth of resources, relationships, and intelligence, all through a single endpoint: `https://graph.microsoft.com`.</span></span>

## <a name="whats-in-the-graph"></a><span data-ttu-id="ca64a-104">Graph 有哪些功能？</span><span class="sxs-lookup"><span data-stu-id="ca64a-104">What's in the graph?</span></span>

<span data-ttu-id="ca64a-p102">Microsoft Graph 由各种资源组成，这些资源通过关系相连接。例如，用户可通过 [memberOf](../api-reference/v1.0/api/user_list_memberof.md) 关系连接到某个组，也可以通过 [manager](../api-reference/v1.0/api/user_list_manager.md) 关系连接到其他用户。你的应用可以遍历这些关系来访问这些连接的资源，并通过 API 对其执行操作。</span><span class="sxs-lookup"><span data-stu-id="ca64a-p102">Microsoft Graph is made up of resources connected by relationships. For example, a user can be connected to a group through a [memberOf](../api-reference/v1.0/api/user_list_memberof.md) relationship, and to another user through a [manager](../api-reference/v1.0/api/user_list_manager.md) relationship. Your app can traverse these relationships to access these connected resources and perform actions on them through the API.</span></span>

<span data-ttu-id="ca64a-p103">还可以从 Microsoft Graph 中获取与数据相关的有价值的见解和情报。例如，你可以获得特定用户[常用的](../api-reference/beta/resources/insights_trending.md)文件，或者获取与用户最为相关的[人员](../api-reference/beta/api/user_list_people.md)。</span><span class="sxs-lookup"><span data-stu-id="ca64a-p103">You can also get valuable insights and intelligence about the data from Microsoft Graph. For example, you can get the popular files [trending around](../api-reference/beta/resources/insights_trending.md) a particular user, or get the most relevant [people](../api-reference/beta/api/user_list_people.md) around a user.</span></span>

<span data-ttu-id="ca64a-110">在 Microsoft Graph 中发现关系的可能性。</span><span class="sxs-lookup"><span data-stu-id="ca64a-110">Discover the possibilities in the relationships within Microsoft Graph.</span></span>

![显示作为 Graph 一部分的主要资源和关系的图片](images/microsoft_graph.png)

## <a name="what-can-you-do-with-microsoft-graph"></a><span data-ttu-id="ca64a-112">可以使用 Microsoft Graph 执行哪些操作？</span><span class="sxs-lookup"><span data-stu-id="ca64a-112">What can you do with Microsoft Graph?</span></span> 

<span data-ttu-id="ca64a-p104">可以使用 Microsoft Graph 为用户构建独特的周围环境体验，帮助他们提高工作效率。假设一个应用可以...</span><span class="sxs-lookup"><span data-stu-id="ca64a-p104">You can use Microsoft Graph to build experiences around the user's unique context to help them be more productive. Imagine an app that...</span></span>

- <span data-ttu-id="ca64a-115">查看下一次会议，并可通过提供与会者的个人资料信息帮助你准备会议，包括他们的职务、工作伙伴以及最近处理的文档和项目信息。</span><span class="sxs-lookup"><span data-stu-id="ca64a-115">Looks at your next meeting and helps you prepare for it by providing profile information for attendees, including their job titles and who they work with, as well as information on the latest documents and projects they're working on.</span></span>
- <span data-ttu-id="ca64a-116">扫描你的日历，并为下一次团队会议提出最佳时间建议。</span><span class="sxs-lookup"><span data-stu-id="ca64a-116">Scans your calendar, and suggests the best times for the next team meeting.</span></span>
- <span data-ttu-id="ca64a-117">从 OneDrive 中的 Excel 文件获取最新销售预测图表，让你可以实时更新趋势预测，这一切通过手机就可以实现。</span><span class="sxs-lookup"><span data-stu-id="ca64a-117">Fetches the latest sales projection chart from an Excel file in your OneDrive and lets you update the forecast in real time, all from your phone.</span></span>
- <span data-ttu-id="ca64a-118">订阅日历更改、当你在会议中花费太长时间发出警报，还可以根据与会者和你的相关性，为可能错过或委托的会议提供建议。</span><span class="sxs-lookup"><span data-stu-id="ca64a-118">Subscribes to changes in your calendar, sends you an alert when you’re spending too much time in meetings, and provides recommendations for the ones you could miss or delegate based on how relevant the attendees are to you.</span></span>
- <span data-ttu-id="ca64a-119">帮助你整理手机上的个人和工作信息；例如，对应当归到个人 OneDrive 的照片和应当归到 OneDrive for Business 的业务收据进行分类。</span><span class="sxs-lookup"><span data-stu-id="ca64a-119">Helps you sort out personal and work information on your phone; for example, by categorizing pictures that should go to your personal OneDrive and business receipts that should go to your OneDrive for Business.</span></span>

<span data-ttu-id="ca64a-120">使用 Microsoft Graph API，你可以实现这些功能及其他更多功能。</span><span class="sxs-lookup"><span data-stu-id="ca64a-120">You can do all this and more with the Microsoft Graph API.</span></span>

><span data-ttu-id="ca64a-121">**注意：**使用 Microsoft Graph API，即表示同意接受 [Microsoft Graph 使用条款](../misc/terms-of-use.md)和 [Microsoft 隐私声明](https://go.microsoft.com/fwlink/?LinkId=521839)。</span><span class="sxs-lookup"><span data-stu-id="ca64a-121">**Note:** When you use the Microsoft Graph API, you agree to the [Microsoft Graph Terms of Use](../misc/terms-of-use.md) and the [Microsoft Privacy Statement](https://go.microsoft.com/fwlink/?LinkId=521839).</span></span>

## <a name="next-steps"></a><span data-ttu-id="ca64a-122">后续步骤</span><span class="sxs-lookup"><span data-stu-id="ca64a-122">Next steps</span></span>

- <span data-ttu-id="ca64a-123">查看某些[精选方案](../concepts/featured_scenarios.md)。</span><span class="sxs-lookup"><span data-stu-id="ca64a-123">Check out some [Featured scenarios](../concepts/featured_scenarios.md).</span></span>
- <span data-ttu-id="ca64a-124">请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的示例请求。</span><span class="sxs-lookup"><span data-stu-id="ca64a-124">Try a sample request in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="ca64a-125">使用[快速入门](https://developer.microsoft.com/graph/quick-start)设置准备运行的示例应用。</span><span class="sxs-lookup"><span data-stu-id="ca64a-125">Use the [quick start](https://developer.microsoft.com/graph/quick-start) to set up a ready-to-run sample app.</span></span>
- <span data-ttu-id="ca64a-126">了解如何在你的应用中[获取身份验证令牌](../concepts/auth_overview.md)。</span><span class="sxs-lookup"><span data-stu-id="ca64a-126">Find out how to [get an auth token](../concepts/auth_overview.md) in your app.</span></span>
- <span data-ttu-id="ca64a-127">开始[使用 API](../concepts/use_the_api.md)。</span><span class="sxs-lookup"><span data-stu-id="ca64a-127">Start [using the API](../concepts/use_the_api.md).</span></span>

## <a name="feedback"></a><span data-ttu-id="ca64a-128">有反馈？</span><span class="sxs-lookup"><span data-stu-id="ca64a-128">Feedback?</span></span>

<span data-ttu-id="ca64a-p105">我们非常重视你的反馈意见。请在 [Stack Overflow](http://stackoverflow.com/questions/tagged/office365+or+microsoftgraph) 上与我们联系。使用 [MicrosoftGraph] 标记出你的问题。</span><span class="sxs-lookup"><span data-stu-id="ca64a-p105">Your feedback is important to us. Connect with us on [Stack Overflow](http://stackoverflow.com/questions/tagged/office365+or+microsoftgraph). Tag your questions with {MicrosoftGraph}.</span></span>

