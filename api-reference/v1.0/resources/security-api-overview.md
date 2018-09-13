# <a name="use-the-microsoft-graph-security-api"></a><span data-ttu-id="134ec-101">使用 Microsoft Graph Security API</span><span class="sxs-lookup"><span data-stu-id="134ec-101">Use the Microsoft Graph API</span></span>

<span data-ttu-id="134ec-102">Microsoft Graph 安全 API 提供统一的接口和架构，与来自 Microsoft 和生态系统合作伙伴的安全解决方案集成。</span><span class="sxs-lookup"><span data-stu-id="134ec-102">The Microsoft Graph Security API provides a unified interface and schema to integrate with security solutions from Microsoft and ecosystem partners.</span></span> <span data-ttu-id="134ec-103">这使客户能够简化安全性操作和更好地防御增加网络威胁。</span><span class="sxs-lookup"><span data-stu-id="134ec-103">This empowers customers to streamline security operations and better defend against increasing cyber threats.</span></span> <span data-ttu-id="134ec-104">Microsoft Graph Security API 可以作为联合的安全聚合服务，用于向所有登记的安全提供程序提交查询以获取聚合响应。</span><span class="sxs-lookup"><span data-stu-id="134ec-104">The Microsoft Graph Security API can be used as a federated security aggregation service to submit queries to all onboarded security providers to get aggregated responses.</span></span> <span data-ttu-id="134ec-105">使用 Microsoft Graph Security API 来构建应用程序，从而：</span><span class="sxs-lookup"><span data-stu-id="134ec-105">Use Microsoft Graph Security API to build applications that:</span></span>

- <span data-ttu-id="134ec-106">合并和关联多个来源的安全警告</span><span class="sxs-lookup"><span data-stu-id="134ec-106">Consolidate and correlate security alerts from multiple sources</span></span>
- <span data-ttu-id="134ec-107">解除上下文数据锁定来告知调查</span><span class="sxs-lookup"><span data-stu-id="134ec-107">Unlock contextual data to inform investigations</span></span>
- <span data-ttu-id="134ec-108">自动化安全操作以提高效率</span><span class="sxs-lookup"><span data-stu-id="134ec-108">Automate security operations for greater efficiency</span></span>
- <span data-ttu-id="134ec-109">提供安全数据的可见性，以启用主动风险管理</span><span class="sxs-lookup"><span data-stu-id="134ec-109">Provide visibility into security data to enable proactive risk management</span></span>

<span data-ttu-id="134ec-110">Microsoft Graph Security API 包括以下主要实体。</span><span class="sxs-lookup"><span data-stu-id="134ec-110">The Microsoft Graph Security API includes the following key entities.</span></span>

## <a name="alerts"></a><span data-ttu-id="134ec-111">警报</span><span class="sxs-lookup"><span data-stu-id="134ec-111">Alerts</span></span>

<span data-ttu-id="134ec-112">警报是客户租户内的潜在安全问题，Microsoft 或合作伙伴安全解决方案已经确定并标记需要操作或通知的安全问题。</span><span class="sxs-lookup"><span data-stu-id="134ec-112">Alerts are potential security issues within a customer's tenant that Microsoft or partner security solutions have identified and are flagged for action or notification.</span></span> <span data-ttu-id="134ec-113">借助 Microsoft Graph Security [alerts](alert.md) 实体，您可以统一并简化跨所有集成解决方案的安全问题。</span><span class="sxs-lookup"><span data-stu-id="134ec-113">With the Microsoft Graph Security [alerts](alert.md) entity, you can unify and streamline security  issues across all integrated solutions.</span></span> <span data-ttu-id="134ec-114">这还允许应用程序关联警报和上下文，从而改进威胁保护和响应。</span><span class="sxs-lookup"><span data-stu-id="134ec-114">This also enables applications to correlate alerts and context to improve threat protection and response.</span></span> <span data-ttu-id="134ec-115">通过缩短调查时间和解决事件的时间，这可解锁安全运营效率。</span><span class="sxs-lookup"><span data-stu-id="134ec-115">These unlock security operational efficiencies by reducing investigation time and time to resolution for incidents.</span></span> <span data-ttu-id="134ec-116">使用警报更新功能，可以通过更新 alerts 实体，跨 Microsoft Graph Security API 集成的不同安全产品和服务同步特定警报的状态。 [ ](alert.md)</span><span class="sxs-lookup"><span data-stu-id="134ec-116">With the alert update capability, you can sync the status of specific alerts across different security products and services that are integrated with the Microsoft Graph Security API by updating your [alerts](alert.md) entity.</span></span>

<span data-ttu-id="134ec-117">Microsoft Graph Security 集成解决方案将收到来自下列安全提供程序的警报：</span><span class="sxs-lookup"><span data-stu-id="134ec-117">Microsoft Graph Security-integrated solutions will receive alerts from the following security providers:</span></span>

- <span data-ttu-id="134ec-118">Azure 安全中心</span><span class="sxs-lookup"><span data-stu-id="134ec-118">Azure AD Identity Protection, Azure Security Center</span></span>
- <span data-ttu-id="134ec-119">Azure Active Directory 标识保护</span><span class="sxs-lookup"><span data-stu-id="134ec-119">Azure Active Directory Identity Protection</span></span>
- <span data-ttu-id="134ec-120">Azure 信息保护</span><span class="sxs-lookup"><span data-stu-id="134ec-120">Azure Information Protection</span></span>
- <span data-ttu-id="134ec-121">Microsoft 云应用程序安全性</span><span class="sxs-lookup"><span data-stu-id="134ec-121">Microsoft Cloud Security Policy</span></span>
- <span data-ttu-id="134ec-122">Windows Defender 高级威胁防护</span><span class="sxs-lookup"><span data-stu-id="134ec-122">Windows Defender Advanced Threat Protection</span></span>
- <span data-ttu-id="134ec-123">Microsoft Intune（个人预览版）</span><span class="sxs-lookup"><span data-stu-id="134ec-123">Microsoft Intune (private preview)</span></span>
- <span data-ttu-id="134ec-124">Office 365（即将推出）</span><span class="sxs-lookup"><span data-stu-id="134ec-124">Office 365 (coming soon)</span></span>
- <span data-ttu-id="134ec-125">合作伙伴解决方案，如 Palo Alto Networks 应用框架</span><span class="sxs-lookup"><span data-stu-id="134ec-125">Partner solutions, such as Palo Alto Networks App Framework</span></span>

> <span data-ttu-id="134ec-126">**注意：** 新的提供程序正加入 Microsoft Graph Security 生态系统。</span><span class="sxs-lookup"><span data-stu-id="134ec-126">**Note:** New providers are continuously onboarding to the Microsoft Graph Security ecosystem.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="134ec-127">常见用例</span><span class="sxs-lookup"><span data-stu-id="134ec-127">Common use cases</span></span>

<span data-ttu-id="134ec-128">下面是一些有关使用 Microsoft Graph Security API 的最常用请求：</span><span class="sxs-lookup"><span data-stu-id="134ec-128">The following are some of the most popular requests for working with the Microsoft Graph Security API:</span></span>

| <span data-ttu-id="134ec-129">**用例**</span><span class="sxs-lookup"><span data-stu-id="134ec-129">**Use cases**</span></span>   | <span data-ttu-id="134ec-130">**REST 资源**</span><span class="sxs-lookup"><span data-stu-id="134ec-130">**REST resources**</span></span> | <span data-ttu-id="134ec-131">**在 Graph 浏览器中试用**</span><span class="sxs-lookup"><span data-stu-id="134ec-131">**Try in Graph Explorer**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="134ec-132">列出警报</span><span class="sxs-lookup"><span data-stu-id="134ec-132">List alerts</span></span> | [<span data-ttu-id="134ec-133">列出警报</span><span class="sxs-lookup"><span data-stu-id="134ec-133">List alerts</span></span>](../api/alert_list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/en-us/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| <span data-ttu-id="134ec-134">更新通知</span><span class="sxs-lookup"><span data-stu-id="134ec-134">Update alerts</span></span> | [<span data-ttu-id="134ec-135">更新警报</span><span class="sxs-lookup"><span data-stu-id="134ec-135">Update alert</span></span>](../api/alert_update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/en-us/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

<span data-ttu-id="134ec-136">您可以使用 Microsoft Graph [webhooks](../../../concepts/webhooks.md) 订阅和接收有关 Microsoft Graph Security 实体的更新通知。</span><span class="sxs-lookup"><span data-stu-id="134ec-136">You can use Microsoft Graph [webhooks](../../../concepts/webhooks.md) to subscribe to and receive notifications about updates to Microsoft Graph Security entities.</span></span>

## <a name="resources"></a><span data-ttu-id="134ec-137">资源</span><span class="sxs-lookup"><span data-stu-id="134ec-137">Resources</span></span>

<span data-ttu-id="134ec-138">代码并参与到这些 Microsoft Graph Security API 示例：</span><span class="sxs-lookup"><span data-stu-id="134ec-138">Code and contribute to these Microsoft Graph Security API samples:</span></span>

- [<span data-ttu-id="134ec-139">ASP.NET (C#) 示例</span><span class="sxs-lookup"><span data-stu-id="134ec-139">ASP.NET (C#) sample</span></span>](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [<span data-ttu-id="134ec-140">Python 示例</span><span class="sxs-lookup"><span data-stu-id="134ec-140">Python Sample</span></span>](https://github.com/microsoftgraph/python-security-rest-sample)
- [<span data-ttu-id="134ec-141">Node.js (JavaScript) 示例</span><span class="sxs-lookup"><span data-stu-id="134ec-141">Node.js (JavaScript) sample</span></span>](https://github.com/microsoftgraph/nodejs-security-sample)

<span data-ttu-id="134ec-142">参与社区：</span><span class="sxs-lookup"><span data-stu-id="134ec-142">Engage with the community:</span></span>

- [<span data-ttu-id="134ec-143">加入技术社区</span><span class="sxs-lookup"><span data-stu-id="134ec-143">Join the tech community</span></span>](https://aka.ms/graphsecuritycommunity)
- [<span data-ttu-id="134ec-144">在 StackOverflow 上讨论</span><span class="sxs-lookup"><span data-stu-id="134ec-144">Discuss on StackOverflow</span></span>](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a><span data-ttu-id="134ec-145">后续步骤</span><span class="sxs-lookup"><span data-stu-id="134ec-145">Next steps</span></span>

<span data-ttu-id="134ec-146">Microsoft Graph Security API 可以打开新的方式，让您可以使用来自 Microsoft 和合作伙伴的不同安全解决方案。</span><span class="sxs-lookup"><span data-stu-id="134ec-146">The Microsoft Graph Security API can open up new ways for you to engage with different security solutions from Microsoft and partners.</span></span> <span data-ttu-id="134ec-147">按照以下步骤开始：</span><span class="sxs-lookup"><span data-stu-id="134ec-147">Follow these steps to get started:</span></span>

- <span data-ttu-id="134ec-148">向下钻取到 [通知](alert.md)。</span><span class="sxs-lookup"><span data-stu-id="134ec-148">Drill down into [alerts](alert.md).</span></span>
- <span data-ttu-id="134ec-149">尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。</span><span class="sxs-lookup"><span data-stu-id="134ec-149">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span> <span data-ttu-id="134ec-150">在**查询示例**下，选择**显示更多示例**，并将安全类别设置为**开**。</span><span class="sxs-lookup"><span data-stu-id="134ec-150">Under **Sample Queries**, choose **show more samples** and set the Security category to **on**.</span></span>
- <span data-ttu-id="134ec-151">尝试在实体更改[订阅和接收通知](../../../concepts/webhooks.md) 。</span><span class="sxs-lookup"><span data-stu-id="134ec-151">Try [subscribing to and receiving notifications](../../../concepts/webhooks.md) on entity changes.</span></span>

<span data-ttu-id="134ec-p105">需要更多想法？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。</span><span class="sxs-lookup"><span data-stu-id="134ec-p105">Need more ideas? See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
