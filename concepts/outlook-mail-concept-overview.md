---
title: Outlook 邮件 API 概述
description: Outlook 是 Microsoft 365 的消息传递通信中心。 使用它，还可以管理联系人、安排会议、查找组织用户的相关信息、
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.custom: scenarios:getting-started
ms.openlocfilehash: 0fcfb1a56e811d7ba63dcd1daed83122132c32bc
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645624"
---
# <a name="outlook-mail-api-overview"></a><span data-ttu-id="ec626-104">Outlook 邮件 API 概述</span><span class="sxs-lookup"><span data-stu-id="ec626-104">Outlook mail API overview</span></span>

<span data-ttu-id="ec626-p102">Outlook 是 Microsoft 365 的消息传递通信中心。有了它，你同样能管理联系人、安排会议、在组织中查找用户相关信息、发起在线对话、共享文件，并实现小组协作。</span><span class="sxs-lookup"><span data-stu-id="ec626-p102">Outlook is a messaging communication hub in Microsoft 365. It also lets you manage contacts, schedule meetings, find information about users in an organization, initiate online conversations, share files, and collaborate in groups.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/L-gm25wusIQ]

## <a name="why-integrate-with-outlook-mail"></a><span data-ttu-id="ec626-107">为什么与 Outlook 邮件集成？</span><span class="sxs-lookup"><span data-stu-id="ec626-107">Why integrate with Outlook mail?</span></span>

### <a name="integrate-with-rich-features-and-reach-hundreds-of-millions-of-customers"></a><span data-ttu-id="ec626-108">与丰富的功能集成进而服务于数以亿计的客户</span><span class="sxs-lookup"><span data-stu-id="ec626-108">Integrate with rich features and reach hundreds of millions of customers</span></span>

<span data-ttu-id="ec626-109">与 Outlook 集成意味着可利用客户所喜爱的丰富体验，即在包括移动、Web 和桌面在内的所有设备上提供的针对邮件、[联系人](outlook-contacts-concept-overview.md)、[日历](outlook-calendar-concept-overview.md)的一致、直观体验。</span><span class="sxs-lookup"><span data-stu-id="ec626-109">Integrating with Outlook means tapping into the rich experience that customers love - consistent, intuitive experience for mail, [contacts](outlook-contacts-concept-overview.md), [calendar](outlook-calendar-concept-overview.md), available on all devices - mobile, web, and desktop.</span></span>

<span data-ttu-id="ec626-110">使用 [Microsoft Graph](overview.md)，你只需编写一个应用与 Outlook 进行集成，即可服务于数以亿计的消费者，以及选择 Outlook 作为其电子邮件客户端的数以千万的组织客户。</span><span class="sxs-lookup"><span data-stu-id="ec626-110">Using [Microsoft Graph](overview.md), you can integrate with Outlook by writing an app just once and reach more than hundreds of millions of consumers, and tens of millions of organization customers who choose Outlook as their email client.</span></span> <span data-ttu-id="ec626-111">你可以编写专注于邮件方案的应用，或连接到大量其他 Outlook 和非 Outlook 关系、资源和智能，并实现 Microsoft 云支持的方案。</span><span class="sxs-lookup"><span data-stu-id="ec626-111">You can write apps that focus on mail scenarios, or connect to a wealth of other Outlook and non-Outlook relationships, resources, and intelligence, and realize scenarios supported by the Microsoft cloud.</span></span>

### <a name="automate-message-organization-and-processing"></a><span data-ttu-id="ec626-112">自动化邮件组织和处理</span><span class="sxs-lookup"><span data-stu-id="ec626-112">Automate message organization and processing</span></span>

<span data-ttu-id="ec626-p104">客户对 Outlook 帮助他们保持井然有序的方式颇为青睐。Microsoft Graph 为应用开发人员提供了这些功能，让他们能够构建可优化发现及提高效率和生产率的客户工作流：</span><span class="sxs-lookup"><span data-stu-id="ec626-p104">Customers like how Outlook helps them stay organized. Microsoft Graph brings these features to app developers, enabling them to build customer workflows that optimize on discovery and improve efficiency and productivity:</span></span>

- <span data-ttu-id="ec626-115">客户会以不同的方式组织他们的邮件，一些客户会将所有邮件都放在收件箱中，只需搜索即可，而有些客户会在文件夹中归档邮件。</span><span class="sxs-lookup"><span data-stu-id="ec626-115">Customers organize their messages in different ways - some leave all messages in the Inbox and simply search for them, others file their messages in folders.</span></span> <span data-ttu-id="ec626-116">他们喜欢 Outlook 这种可支持扁平式组织和基于文件夹组织的灵活又直观的方法。</span><span class="sxs-lookup"><span data-stu-id="ec626-116">They like Outlook's flexible and intuitive approach that supports both flat and folder-based organizations.</span></span> <span data-ttu-id="ec626-117">应用可以方便地对特定文件夹或用户整个邮箱中的邮件进行[筛选、搜索或排序](query-parameters.md)。</span><span class="sxs-lookup"><span data-stu-id="ec626-117">Apps can conveniently [filter, search, or sort](query-parameters.md) messages in specific folders or the user's entire mailbox.</span></span>

- <span data-ttu-id="ec626-118">Outlook 类别按名称和颜色进行区分。</span><span class="sxs-lookup"><span data-stu-id="ec626-118">Outlook categories are differentiated by name and color.</span></span> <span data-ttu-id="ec626-119">客户可使用类别标记邮件，以增强组织和发现。</span><span class="sxs-lookup"><span data-stu-id="ec626-119">Categories allow customers to tag messages to enhance organization and discovery.</span></span> <span data-ttu-id="ec626-120">应用可以访问和[定义用户的主类别列表](/graph/api/outlookuser-post-mastercategories)。</span><span class="sxs-lookup"><span data-stu-id="ec626-120">Apps can access and [define a user's master list of categories](/graph/api/outlookuser-post-mastercategories).</span></span> <span data-ttu-id="ec626-121">此外，该列表可在 Outlook 邮件，以及事件、联系人、任务和组文章中进行共享，为应用开发者开启了创造性的应用场景。</span><span class="sxs-lookup"><span data-stu-id="ec626-121">More, that list is shared across Outlook messages, as well as events, contacts, tasks, and group posts, and opens up creative scenarios for app developers.</span></span> <span data-ttu-id="ec626-122">例如，在线培训提供商可以为电子邮件、课程事件设置颜色代码，并跟进用户已注册的各课程的后续作业。</span><span class="sxs-lookup"><span data-stu-id="ec626-122">For example, an online training provider can color-code the emails, course events, and follow-up assignments for each course a user has enrolled in.</span></span>

- <span data-ttu-id="ec626-123">此外，应用用户还可更改邮件（或事件或任务）的重要性，或标记邮件以供后续跟进。</span><span class="sxs-lookup"><span data-stu-id="ec626-123">Additionally, app users can change the importance of a message (or event or task), or flag a message for follow-up.</span></span> <span data-ttu-id="ec626-124">（Microsoft Graph 中的标记目前为[预览状态](versioning-and-support.md#beta-version)。）</span><span class="sxs-lookup"><span data-stu-id="ec626-124">(Flagging is currently [in preview](versioning-and-support.md#beta-version) in Microsoft Graph.)</span></span>

- <span data-ttu-id="ec626-125">规则 API 将邮件组织提升到了一个新的水平。</span><span class="sxs-lookup"><span data-stu-id="ec626-125">The rules API takes message organization to the next level.</span></span> <span data-ttu-id="ec626-126">应用可以设置[收件箱规则](/graph/api/resources/messagerule)，以尽快处理传入的邮件并减少电子邮件混乱。</span><span class="sxs-lookup"><span data-stu-id="ec626-126">Apps can set up [Inbox rules](/graph/api/resources/messagerule) to promptly handle incoming messages and reduce email clutter.</span></span> <span data-ttu-id="ec626-127">例如，如果邮件主题行包含某些关键字，则应用可以自动将邮件移动到另一个文件夹，并分配类别和重要性，使其易于后续跟进。</span><span class="sxs-lookup"><span data-stu-id="ec626-127">For example, an app can automatically move messages to another folder if their subject lines contain certain keywords, and assign categories and importance to make them easier for later follow-up.</span></span>

- <span data-ttu-id="ec626-128">许多客户使用采用 MIME 格式发送和接收邮件的电子邮件客户端。</span><span class="sxs-lookup"><span data-stu-id="ec626-128">Many customers use email clients that send and receive messages in MIME format.</span></span> <span data-ttu-id="ec626-129">即使 Outlook 不会以 MIME 格式保存邮件，应用也可以[以 MIME 格式获取 Outlook 邮件正文](outlook-get-mime-message.md)，[以 MIME 格式发送 Outlook 邮件](outlook-send-mime-message.md)，附加 S/MIME 数字签名，并以 S/MIME 加密邮件内容。</span><span class="sxs-lookup"><span data-stu-id="ec626-129">Even though Outlook does not save messages in MIME format, apps can [get the body of an Outlook message in MIME format](outlook-get-mime-message.md), [send Outlook messages in MIME format](outlook-send-mime-message.md), attach S/MIME digital signatures, and encrypt message content in S/MIME.</span></span>

### <a name="write-smarter-apps-that-leverage-intelligence"></a><span data-ttu-id="ec626-130">编写利用智能的更智能应用</span><span class="sxs-lookup"><span data-stu-id="ec626-130">Write smarter apps that leverage intelligence</span></span>

<span data-ttu-id="ec626-131">使用 Microsoft Graph 向应用用户建议上下文数据：</span><span class="sxs-lookup"><span data-stu-id="ec626-131">Use Microsoft Graph to suggest contextual data to your app users:</span></span>

- <span data-ttu-id="ec626-132">与[重点收件箱](/graph/api/resources/manage-focused-inbox)和 [@提及（预览版）](/graph/api/message-get?view=graph-rest-beta&preserve-view=true#example-2-get-all-mentions-in-a-specific-message)集成，让应用用户能够先阅读和答复与自己相关的邮件。</span><span class="sxs-lookup"><span data-stu-id="ec626-132">Integrate with [Focused Inbox](/graph/api/resources/manage-focused-inbox) and [@-mentions (preview)](/graph/api/message-get?view=graph-rest-beta&preserve-view=true#example-2-get-all-mentions-in-a-specific-message) and let your app users read and respond to what's relevant to them first.</span></span>

- <span data-ttu-id="ec626-133">一边查看[邮件提示](/graph/api/resources/mailtips)，一边仍能撰写邮件，以获取收件人的实用状态信息（如收件人正在发送自动答复或邮箱已满）。</span><span class="sxs-lookup"><span data-stu-id="ec626-133">Check [mail tips](/graph/api/resources/mailtips) while still composing a message to get useful status information about a recipient (such as the recipient sending an auto-reply or has a full mailbox).</span></span> <span data-ttu-id="ec626-134">邮件提示可以提醒应用注意特定条件，以便采取更高效的跟进操作。</span><span class="sxs-lookup"><span data-stu-id="ec626-134">Mail tips can alert apps of certain conditions so to take more efficient follow-up actions instead.</span></span>

- <span data-ttu-id="ec626-135">使用[人员 API](people-example.md) 提供交互式控件，如应用中的人员选取器。</span><span class="sxs-lookup"><span data-stu-id="ec626-135">Make use of the [people API](people-example.md) to provide interactive controls such as a people picker in your app.</span></span> <span data-ttu-id="ec626-136">人员 API 可根据用户通信和协作模式及业务关系建议与用户相关度最高的人员。</span><span class="sxs-lookup"><span data-stu-id="ec626-136">The people API can suggest persons most relevant to a user, based on the user’s communication and collaboration patterns and business relationships.</span></span>

- <span data-ttu-id="ec626-137">为应用用户提供智能文件选取器并建议他们最近与之交互的文件，以便在撰写邮件时以附件形式添加。</span><span class="sxs-lookup"><span data-stu-id="ec626-137">Offer app users a smart file picker and suggest files that they have recently interacted with, to add as attachments when composing a message.</span></span> <span data-ttu-id="ec626-138">[见解](/graph/api/resources/officegraphinsights)使用高级分析来推荐用户有可能使用的文件、用户最近查看或编辑的文件，或者与用户共享的文件。</span><span class="sxs-lookup"><span data-stu-id="ec626-138">[Insights](/graph/api/resources/officegraphinsights) use advanced analytics to suggest files that are trending around a user, recently viewed or edited by the user, or shared with the user.</span></span>


### <a name="store-app-data-in-a-resource-or-resource-instance"></a><span data-ttu-id="ec626-139">在资源或资源实例中存储应用数据</span><span class="sxs-lookup"><span data-stu-id="ec626-139">Store app data in a resource or resource instance</span></span>

<span data-ttu-id="ec626-140">大部分情况下，应用需要将数据存储在外部数据存储中，并承担数据管理和访问开销。</span><span class="sxs-lookup"><span data-stu-id="ec626-140">Often times apps have to store their data in an external data store and entail overhead in managing and accessing the data.</span></span> <span data-ttu-id="ec626-141">借助 Microsoft Graph，可以在[创建](/graph/api/user-post-messages#example-2-create-message-draft-that-includes-custom-message-headers)或[发送](/graph/api/user-sendmail#example-2-create-a-message-with-custom-internet-message-headers-and-send-the-message)新邮件或邮件回复时，直接将应用数据添加为 Internet 邮件头。</span><span class="sxs-lookup"><span data-stu-id="ec626-141">Microsoft Graph lets you simply include app data as Internet message headers when [creating](/graph/api/user-post-messages#example-2-create-message-draft-that-includes-custom-message-headers) or [sending](/graph/api/user-sendmail#example-2-create-a-message-with-custom-internet-message-headers-and-send-the-message) a new message, or a reply to a message.</span></span>

<span data-ttu-id="ec626-142">如果需要添加并随后更新自定义数据，可以[在各个资源实例中存储数据](extensibility-overview.md#open-extensions)。</span><span class="sxs-lookup"><span data-stu-id="ec626-142">If you need to add and subsequently update custom data, you can [store the data in individual resource instances](extensibility-overview.md#open-extensions).</span></span> <span data-ttu-id="ec626-143">也可以在适当情况下扩展架构、添加自定义属性，并在 Microsoft Graph 资源中存储类型化数据。</span><span class="sxs-lookup"><span data-stu-id="ec626-143">If appropriate, as an alternative, you can extend the schema, add custom properties, and store typed data in Microsoft Graph resources.</span></span> <span data-ttu-id="ec626-144">可以让此类[架构扩展](extensibility-overview.md#schema-extensions)可供发现和共享。</span><span class="sxs-lookup"><span data-stu-id="ec626-144">You can make such [schema extensions](extensibility-overview.md#schema-extensions) discoverable and shareable.</span></span>

## <a name="where-is-the-data"></a><span data-ttu-id="ec626-145">数据在什么位置？</span><span class="sxs-lookup"><span data-stu-id="ec626-145">Where is the data?</span></span>

[!INCLUDE [outlook-mailbox-type-support](../includes/outlook-mailbox-type-support.md)]

## <a name="api-reference"></a><span data-ttu-id="ec626-146">API 参考</span><span class="sxs-lookup"><span data-stu-id="ec626-146">API reference</span></span>
<span data-ttu-id="ec626-147">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="ec626-147">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="ec626-148">Microsoft Graph v1.0 中的 Outlook 邮件 API</span><span class="sxs-lookup"><span data-stu-id="ec626-148">Outlook mail API in Microsoft Graph v1.0</span></span>](/graph/api/resources/mail-api-overview)
- [<span data-ttu-id="ec626-149">Microsoft Graph beta 中的 Outlook 邮件 API</span><span class="sxs-lookup"><span data-stu-id="ec626-149">Outlook mail API in Microsoft Graph beta</span></span>](/graph/api/resources/mail-api-overview?view=graph-rest-beta&preserve-view=true)


## <a name="next-steps"></a><span data-ttu-id="ec626-150">后续步骤</span><span class="sxs-lookup"><span data-stu-id="ec626-150">Next steps</span></span>

- <span data-ttu-id="ec626-151">在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0)中选择和试用 Outlook 邮件示例查询。</span><span class="sxs-lookup"><span data-stu-id="ec626-151">Select and try Outlook mail sample queries in [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0).</span></span> <span data-ttu-id="ec626-152">选择左侧列中的“显示更多示例”。</span><span class="sxs-lookup"><span data-stu-id="ec626-152">Choose **Show more samples** in the column on the left.</span></span> <span data-ttu-id="ec626-153">使用菜单打开“Outlook 邮件”。</span><span class="sxs-lookup"><span data-stu-id="ec626-153">Use the menu to turn on **Outlook Mail**.</span></span>
- <span data-ttu-id="ec626-154">了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="ec626-154">Learn about:</span></span>

  - [<span data-ttu-id="ec626-155">创建和发送邮件</span><span class="sxs-lookup"><span data-stu-id="ec626-155">Creating and sending messages</span></span>](outlook-create-send-messages.md)
  - <span data-ttu-id="ec626-156">[邮件整理](outlook-organize-messages.md)方法</span><span class="sxs-lookup"><span data-stu-id="ec626-156">Ways to [organize messages](outlook-organize-messages.md)</span></span>
  - [<span data-ttu-id="ec626-157">获取邮件的 MIME 内容</span><span class="sxs-lookup"><span data-stu-id="ec626-157">Getting the MIME content of a message</span></span>](outlook-get-mime-message.md)
  - [<span data-ttu-id="ec626-158">将大文件附加到 Outlook 邮件或事件</span><span class="sxs-lookup"><span data-stu-id="ec626-158">Attaching large files to Outlook messages or events</span></span>](outlook-large-attachments.md)
  - [<span data-ttu-id="ec626-159">获取共享邮件</span><span class="sxs-lookup"><span data-stu-id="ec626-159">Getting shared messages</span></span>](outlook-share-messages-folders.md)
  - <span data-ttu-id="ec626-160">如何[从其他用户身份发送邮件](outlook-send-mail-from-other-user.md)</span><span class="sxs-lookup"><span data-stu-id="ec626-160">How to [send mail from another user](outlook-send-mail-from-other-user.md)</span></span>
  - [<span data-ttu-id="ec626-161">获取 Outlook 资源的不可变标识符</span><span class="sxs-lookup"><span data-stu-id="ec626-161">Getting immutable identifiers for Outlook resources</span></span>](outlook-immutable-id.md)
  - [<span data-ttu-id="ec626-162">发送含有 MIME 内容的电子邮件</span><span class="sxs-lookup"><span data-stu-id="ec626-162">Sending emails with MIME contents</span></span>](outlook-send-mime-message.md)

- <span data-ttu-id="ec626-163">详细了解如何使用 Microsoft Graph v1.0 中的[邮件 API](/graph/api/resources/mail-api-overview) 及其[用例](/graph/api/resources/mail-api-overview#common-use-cases)。</span><span class="sxs-lookup"><span data-stu-id="ec626-163">Find out more about [using the mail API](/graph/api/resources/mail-api-overview) and its [use cases](/graph/api/resources/mail-api-overview#common-use-cases) in Microsoft Graph v1.0.</span></span>


