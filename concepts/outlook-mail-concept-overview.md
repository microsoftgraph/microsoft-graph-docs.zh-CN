---
title: Outlook 邮件 API 概述
description: Outlook 是 Microsoft 365 的消息传递通信中心。 使用它，还可以管理联系人、安排会议、查找组织用户的相关信息、
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.custom: scenarios:getting-started
ms.openlocfilehash: 0a9c5d5a84c54a733283ae40c1f70d2670bb7b36
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895522"
---
# <a name="outlook-mail-api-overview"></a><span data-ttu-id="cb7ea-104">Outlook 邮件 API 概述</span><span class="sxs-lookup"><span data-stu-id="cb7ea-104">Outlook mail API overview</span></span>

<span data-ttu-id="cb7ea-105">Outlook 是 Microsoft 365 的消息传递通信中心。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-105">Outlook is a messaging communication hub in Microsoft 365.</span></span> <span data-ttu-id="cb7ea-106">有了它，你同样能管理联系人、安排会议、在组织中查找用户相关信息、发起在线对话、共享文件，并实现小组协作。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-106">It also lets you manage contacts, schedule meetings, find information about users in an organization, initiate online conversations, share files, and collaborate in groups.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/L-gm25wusIQ]

## <a name="why-integrate-with-outlook-mail"></a><span data-ttu-id="cb7ea-107">为什么与 Outlook 邮件集成？</span><span class="sxs-lookup"><span data-stu-id="cb7ea-107">Why integrate with Outlook mail?</span></span>

### <a name="integrate-with-rich-features-and-reach-hundreds-of-millions-of-customers"></a><span data-ttu-id="cb7ea-108">与丰富的功能集成进而服务于数以亿计的客户</span><span class="sxs-lookup"><span data-stu-id="cb7ea-108">Integrate with rich features and reach hundreds of millions of customers</span></span>

<span data-ttu-id="cb7ea-109">与 Outlook 集成意味着可利用客户所喜爱的丰富体验，即在包括移动、Web 和桌面在内的所有设备上提供的针对邮件、[联系人](outlook-contacts-concept-overview.md)、[日历](outlook-calendar-concept-overview.md)的一致、直观体验。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-109">Integrating with Outlook means tapping into the rich experience that customers love - consistent, intuitive experience for mail, [contacts](outlook-contacts-concept-overview.md), [calendar](outlook-calendar-concept-overview.md), available on all devices - mobile, web, and desktop.</span></span>

<span data-ttu-id="cb7ea-110">使用 [Microsoft Graph](overview.md)，你只需编写一个应用与 Outlook 进行集成，即可服务于数以亿计的消费者，以及选择 Outlook 作为其电子邮件客户端的数以千万的组织客户。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-110">Using [Microsoft Graph](overview.md), you can integrate with Outlook by writing an app just once and reach more than hundreds of millions of consumers, and tens of millions of organization customers who choose Outlook as their email client.</span></span> <span data-ttu-id="cb7ea-111">你可以编写专注于邮件方案的应用，或连接到大量其他 Outlook 和非 Outlook 关系、资源和智能，并实现 Microsoft 云支持的方案。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-111">You can write apps that focus on mail scenarios, or connect to a wealth of other Outlook and non-Outlook relationships, resources, and intelligence, and realize scenarios supported by the Microsoft cloud.</span></span>

### <a name="automate-message-organization-and-processing"></a><span data-ttu-id="cb7ea-112">自动化邮件组织和处理</span><span class="sxs-lookup"><span data-stu-id="cb7ea-112">Automate message organization and processing</span></span>

<span data-ttu-id="cb7ea-113">客户对 Outlook 帮助他们保持井然有序的方式颇为青睐。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-113">Customers like how Outlook helps them stay organized.</span></span> <span data-ttu-id="cb7ea-114">Microsoft Graph 为应用开发人员提供了这些功能，让他们能够构建可优化发现及提高效率和生产率的客户工作流：</span><span class="sxs-lookup"><span data-stu-id="cb7ea-114">Microsoft Graph brings these features to app developers, enabling them to build customer workflows that optimize on discovery and improve efficiency and productivity:</span></span>

- <span data-ttu-id="cb7ea-115">客户会以不同的方式组织他们的邮件，一些客户会将所有邮件都放在收件箱中，只需搜索即可，而有些客户会在文件夹中归档邮件。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-115">Customers organize their messages in different ways - some leave all messages in the Inbox and simply search for them, others file their messages in folders.</span></span> <span data-ttu-id="cb7ea-116">他们喜欢 Outlook 这种可支持扁平式组织和基于文件夹组织的灵活又直观的方法。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-116">They like Outlook's flexible and intuitive approach that supports both flat and folder-based organizations.</span></span> <span data-ttu-id="cb7ea-117">应用可以方便地对特定文件夹或用户整个邮箱中的邮件进行[筛选、搜索或排序](query-parameters.md)。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-117">Apps can conveniently [filter, search, or sort](query-parameters.md) messages in specific folders or the user's entire mailbox.</span></span>

- <span data-ttu-id="cb7ea-118">Outlook 类别按名称和颜色进行区分。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-118">Outlook categories are differentiated by name and color.</span></span> <span data-ttu-id="cb7ea-119">客户可使用类别标记邮件，以增强组织和发现。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-119">Categories allow customers to tag messages to enhance organization and discovery.</span></span> <span data-ttu-id="cb7ea-120">应用可以访问和[定义用户的主类别列表](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-120">Apps can access and [define a user's master list of categories](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0).</span></span> <span data-ttu-id="cb7ea-121">此外，该列表可在 Outlook 邮件，以及事件、联系人、任务和组文章中进行共享，为应用开发者开启了创造性的应用场景。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-121">More, that list is shared across Outlook messages, as well as events, contacts, tasks, and group posts, and opens up creative scenarios for app developers.</span></span> <span data-ttu-id="cb7ea-122">例如，在线培训提供商可以为电子邮件、课程事件设置颜色代码，并跟进用户已注册的各课程的后续作业。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-122">For example, an online training provider can color-code the emails, course events, and follow-up assignments for each course a user has enrolled in.</span></span>

- <span data-ttu-id="cb7ea-123">此外，应用用户还可更改邮件（或事件或任务）的重要性，或标记邮件以供后续跟进。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-123">Additionally, app users can change the importance of a message (or event or task), or flag a message for follow-up.</span></span> <span data-ttu-id="cb7ea-124">（Microsoft Graph 中的标记目前为[预览状态](versioning-and-support.md#beta-version)。）</span><span class="sxs-lookup"><span data-stu-id="cb7ea-124">(Flagging is currently [in preview](versioning-and-support.md#beta-version) in Microsoft Graph.)</span></span>

- <span data-ttu-id="cb7ea-125">规则 API 将邮件组织提升到了一个新的水平。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-125">The rules API takes message organization to the next level.</span></span> <span data-ttu-id="cb7ea-126">应用可以设置[收件箱规则](/graph/api/resources/messagerule?view=graph-rest-1.0)，以尽快处理传入的邮件并减少电子邮件混乱。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-126">Apps can set up [Inbox rules](/graph/api/resources/messagerule?view=graph-rest-1.0) to promptly handle incoming messages and reduce email clutter.</span></span> <span data-ttu-id="cb7ea-127">例如，如果邮件主题行包含某些关键字，则应用可以自动将邮件移动到另一个文件夹，并分配类别和重要性，使其易于后续跟进。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-127">For example, an app can automatically move messages to another folder if their subject lines contain certain keywords, and assign categories and importance to make them easier for later follow-up.</span></span>

### <a name="write-smarter-apps-that-leverage-intelligence"></a><span data-ttu-id="cb7ea-128">编写利用智能的更智能应用</span><span class="sxs-lookup"><span data-stu-id="cb7ea-128">Write smarter apps that leverage intelligence</span></span>

<span data-ttu-id="cb7ea-129">使用 Microsoft Graph 向应用用户建议上下文数据：</span><span class="sxs-lookup"><span data-stu-id="cb7ea-129">Use Microsoft Graph to suggest contextual data to your app users:</span></span>

- <span data-ttu-id="cb7ea-130">与[重点收件箱](/graph/api/resources/manage-focused-inbox?view=graph-rest-1.0)和 [@提及（预览版）](/graph/api/message-get?view=graph-rest-beta#request-2)集成，让应用用户能够先阅读和答复与自己相关的邮件。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-130">Integrate with [Focused Inbox](/graph/api/resources/manage-focused-inbox?view=graph-rest-1.0) and [@-mentions (preview)](/graph/api/message-get?view=graph-rest-beta#request-2) and let your app users read and respond to what's relevant to them first.</span></span>

- <span data-ttu-id="cb7ea-131">一边查看[邮件提示](/graph/api/resources/mailtips?view=graph-rest-1.0)，一边仍能撰写邮件，以获取收件人的实用状态信息（如收件人正在发送自动答复或邮箱已满）。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-131">Check [mail tips](/graph/api/resources/mailtips?view=graph-rest-1.0) while still composing a message to get useful status information about a recipient (such as the recipient sending an auto-reply or has a full mailbox).</span></span> <span data-ttu-id="cb7ea-132">邮件提示可以提醒应用注意特定条件，以便采取更高效的跟进操作。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-132">Mail tips can alert apps of certain conditions so to take more efficient follow-up actions instead.</span></span>

- <span data-ttu-id="cb7ea-133">使用[人员 API](people-example.md) 提供交互式控件，如应用中的人员选取器。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-133">Make use of the [people API](people-example.md) to provide interactive controls such as a people picker in your app.</span></span> <span data-ttu-id="cb7ea-134">人员 API 可根据用户通信和协作模式及业务关系建议与用户相关度最高的人员。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-134">The people API can suggest persons most relevant to a user, based on the user’s communication and collaboration patterns and business relationships.</span></span>

- <span data-ttu-id="cb7ea-135">为应用用户提供智能文件选取器并建议他们最近与之交互的文件，以便在撰写邮件时以附件形式添加。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-135">Offer app users a smart file picker and suggest files that they have recently interacted with, to add as attachments when composing a message.</span></span> <span data-ttu-id="cb7ea-136">[见解（预览版）](/graph/api/resources/insights?view=graph-rest-beta)使用高级分析来推荐用户有可能使用的文件、用户最近查看或编辑过的文件或与用户共享的文件。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-136">[Insights (preview)](/graph/api/resources/insights?view=graph-rest-beta) use advanced analytics to suggest files that are trending around a user, recently viewed or edited by the user, or shared with the user.</span></span>


### <a name="store-app-data-in-a-resource-or-resource-instance"></a><span data-ttu-id="cb7ea-137">在资源或资源实例中存储应用数据</span><span class="sxs-lookup"><span data-stu-id="cb7ea-137">Store app data in a resource or resource instance</span></span>

<span data-ttu-id="cb7ea-138">大部分情况下，应用需要将数据存储在外部数据存储中，并承担数据管理和访问开销。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-138">Often times apps have to store their data in an external data store and entail overhead in managing and accessing the data.</span></span> <span data-ttu-id="cb7ea-139">借助 Microsoft Graph，可以在[创建](/graph/api/user-post-messages?view=graph-rest-1.0#request-2)或[发送](/graph/api/user-sendmail?view=graph-rest-1.0#request-2)新邮件或邮件回复时，直接将应用数据添加为 Internet 邮件头。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-139">Microsoft Graph lets you simply include app data as Internet message headers when [creating](/graph/api/user-post-messages?view=graph-rest-1.0#request-2) or [sending](/graph/api/user-sendmail?view=graph-rest-1.0#request-2) a new message, or a reply to a message.</span></span>

<span data-ttu-id="cb7ea-140">如果需要添加并随后更新自定义数据，可以[在各个资源实例中存储数据](extensibility-overview.md#open-extensions)。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-140">If you need to add and subsequently update custom data, you can [store the data in individual resource instances](extensibility-overview.md#open-extensions).</span></span> <span data-ttu-id="cb7ea-141">也可以在适当情况下扩展架构、添加自定义属性，并在 Microsoft Graph 资源中存储类型化数据。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-141">If appropriate, as an alternative, you can extend the schema, add custom properties, and store typed data in Microsoft Graph resources.</span></span> <span data-ttu-id="cb7ea-142">可以让此类[架构扩展](extensibility-overview.md#schema-extensions)可供发现和共享。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-142">You can make such [schema extensions](extensibility-overview.md#schema-extensions) discoverable and shareable.</span></span>

## <a name="where-is-the-data"></a><span data-ttu-id="cb7ea-143">数据在什么位置？</span><span class="sxs-lookup"><span data-stu-id="cb7ea-143">Where is the data?</span></span>

[!INCLUDE [outlook-mailbox-type-support](../includes/outlook-mailbox-type-support.md)]

## <a name="api-reference"></a><span data-ttu-id="cb7ea-144">API 参考</span><span class="sxs-lookup"><span data-stu-id="cb7ea-144">API reference</span></span>
<span data-ttu-id="cb7ea-145">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="cb7ea-145">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="cb7ea-146">Microsoft Graph v1.0 中的 Outlook 邮件 API</span><span class="sxs-lookup"><span data-stu-id="cb7ea-146">Outlook mail API in Microsoft Graph v1.0</span></span>](/graph/api/resources/mail-api-overview?view=graph-rest-1.0)
- [<span data-ttu-id="cb7ea-147">Microsoft Graph beta 中的 Outlook 邮件 API</span><span class="sxs-lookup"><span data-stu-id="cb7ea-147">Outlook mail API in Microsoft Graph beta</span></span>](/graph/api/resources/mail-api-overview?view=graph-rest-beta)


## <a name="next-steps"></a><span data-ttu-id="cb7ea-148">后续步骤</span><span class="sxs-lookup"><span data-stu-id="cb7ea-148">Next steps</span></span>

- <span data-ttu-id="cb7ea-149">在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0)中选择和试用 Outlook 邮件示例查询。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-149">Select and try Outlook mail sample queries in [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0).</span></span> <span data-ttu-id="cb7ea-150">选择左侧列中的“显示更多示例”。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-150">Choose **Show more samples** in the column on the left.</span></span> <span data-ttu-id="cb7ea-151">使用菜单打开“Outlook 邮件”。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-151">Use the menu to turn on **Outlook Mail**.</span></span>
- <span data-ttu-id="cb7ea-152">了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="cb7ea-152">Learn about:</span></span>

  - [<span data-ttu-id="cb7ea-153">创建和发送邮件</span><span class="sxs-lookup"><span data-stu-id="cb7ea-153">Creating and sending messages</span></span>](outlook-create-send-messages.md)
  - <span data-ttu-id="cb7ea-154">[邮件整理](outlook-organize-messages.md)方法</span><span class="sxs-lookup"><span data-stu-id="cb7ea-154">Ways to [organize messages](outlook-organize-messages.md)</span></span>
  - [<span data-ttu-id="cb7ea-155">获取邮件的 MIME 内容</span><span class="sxs-lookup"><span data-stu-id="cb7ea-155">Getting the MIME content of a message</span></span>](outlook-get-mime-message.md)
  - [<span data-ttu-id="cb7ea-156">将大文件附加到 Outlook 邮件或事件</span><span class="sxs-lookup"><span data-stu-id="cb7ea-156">Attaching large files to Outlook messages or events</span></span>](outlook-large-attachments.md)
  - [<span data-ttu-id="cb7ea-157">获取共享邮件</span><span class="sxs-lookup"><span data-stu-id="cb7ea-157">Getting shared messages</span></span>](outlook-share-messages-folders.md)
  - <span data-ttu-id="cb7ea-158">如何[从其他用户身份发送邮件](outlook-send-mail-from-other-user.md)</span><span class="sxs-lookup"><span data-stu-id="cb7ea-158">How to [send mail from another user](outlook-send-mail-from-other-user.md)</span></span>
  - [<span data-ttu-id="cb7ea-159">获取 Outlook 资源的不可变标识符</span><span class="sxs-lookup"><span data-stu-id="cb7ea-159">Getting immutable identifiers for Outlook resources</span></span>](outlook-immutable-id.md)

- <span data-ttu-id="cb7ea-160">详细了解如何使用 Microsoft Graph v1.0 中的[邮件 API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) 及其[用例](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)。</span><span class="sxs-lookup"><span data-stu-id="cb7ea-160">Find out more about [using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>


