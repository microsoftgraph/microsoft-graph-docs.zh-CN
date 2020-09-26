---
title: 云通信 API 概述
description: Microsoft Graph 中的云通信 Api 为您的应用和服务如何通过各种通信相关功能（如呼叫和联机会议）与用户进行交互，从而添加了一个新的维度。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: e672b58d32f0f841aedcf5b639c4d05e15ce582d
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289412"
---
# <a name="cloud-communications-api-overview"></a><span data-ttu-id="71b21-103">云通信 API 概述</span><span class="sxs-lookup"><span data-stu-id="71b21-103">Cloud communications API overview</span></span>
<span data-ttu-id="71b21-104">Microsoft Graph 中的云通信 Api 为您的应用和服务如何通过各种通信相关功能（如呼叫和联机会议）与用户进行交互，从而添加了一个新的维度。</span><span class="sxs-lookup"><span data-stu-id="71b21-104">The cloud communications APIs in Microsoft Graph add a new dimension to how your apps and services interact with users through various communications related features, such as calling and online meetings.</span></span> <span data-ttu-id="71b21-105">通过加快您对客户需求的响应方式以及员工相互协作的方式来扩大业务。</span><span class="sxs-lookup"><span data-stu-id="71b21-105">Grow your business by expediting how you respond to your customers’ needs and how your employees collaborate with each other.</span></span>

## <a name="why-integrate-with-the-cloud-communications-apis"></a><span data-ttu-id="71b21-106">为什么要与云通信 Api 集成？</span><span class="sxs-lookup"><span data-stu-id="71b21-106">Why integrate with the cloud communications APIs?</span></span>

<span data-ttu-id="71b21-107">了解使用云通信 Api 对 buid 服务应用程序 ([bot](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html?q=create%20bot)) 的好处。</span><span class="sxs-lookup"><span data-stu-id="71b21-107">Discover the benefits of using cloud communications APIs to buid service applications ([bots](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html?q=create%20bot)).</span></span>

### <a name="handle-incoming-calls"></a><span data-ttu-id="71b21-108">处理传入呼叫</span><span class="sxs-lookup"><span data-stu-id="71b21-108">Handle incoming calls</span></span>

<span data-ttu-id="71b21-109">当工作人员收到大量业务呼叫且无法回答所有问题时，可能会非常困难。</span><span class="sxs-lookup"><span data-stu-id="71b21-109">It can be overwhelming at times when workers receive a lot of business calls and it isn't possible, or productive, to answer all of them.</span></span> <span data-ttu-id="71b21-110">Bot 可用作前台助理，并通过拒绝似乎像垃圾邮件呼叫那样来处理这些呼叫，然后重定向 (转发) 对不同号码的特定呼叫。</span><span class="sxs-lookup"><span data-stu-id="71b21-110">A bot can serve as a front-desk assistant and handle these calls by rejecting what seem like spam calls, and redirecting (forwarding) specific calls to a different number.</span></span>

<span data-ttu-id="71b21-111">您可以使用云通信 Api 执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="71b21-111">You can use the cloud communications APIs to:</span></span>

- <span data-ttu-id="71b21-112">让用户通过 VoIP [呼叫机器人](/graph/api/application-post-calls?view=graph-rest-1.0) 。</span><span class="sxs-lookup"><span data-stu-id="71b21-112">Have a user [call a bot](/graph/api/application-post-calls?view=graph-rest-1.0) through VoIP.</span></span>
- <span data-ttu-id="71b21-113">如果需要，请让 bot 将 [传入呼叫重定向](/graph/api/call-redirect?view=graph-rest-1.0) 到相应的代理。</span><span class="sxs-lookup"><span data-stu-id="71b21-113">Have a bot [redirect the incoming call](/graph/api/call-redirect?view=graph-rest-1.0) to the appropriate agent if necessary.</span></span>
- <span data-ttu-id="71b21-114">有机器人 [应答](/graph/api/call-answer?view=graph-rest-1.0) 或 [拒绝](/graph/api/call-reject?view=graph-rest-1.0) 呼叫。</span><span class="sxs-lookup"><span data-stu-id="71b21-114">Have a bot [answer](/graph/api/call-answer?view=graph-rest-1.0) or [reject](/graph/api/call-reject?view=graph-rest-1.0) the call.</span></span>


### <a name="simplify-the-customer-service-experience"></a><span data-ttu-id="71b21-115">简化客户服务体验</span><span class="sxs-lookup"><span data-stu-id="71b21-115">Simplify the customer service experience</span></span>
<span data-ttu-id="71b21-116">无论您是拥有一家大型支持服务还是小型店面，都可能很难处理多个客户请求，尤其是在您没有任何上下文正在尝试提前解决的问题时。</span><span class="sxs-lookup"><span data-stu-id="71b21-116">Whether you own a large helpdesk service or a small storefront, it can be difficult to handle multiple customer requests, especially if you don’t have any context of what problem they’re trying to solve beforehand.</span></span> <span data-ttu-id="71b21-117">通过 **交互式语音响应** 处理来自客户的传入呼叫 (IVR) 系统，机器人最初将与之交互。</span><span class="sxs-lookup"><span data-stu-id="71b21-117">Handle incoming calls from customers through an **Interactive Voice Response** (IVR) system, where a bot will initially interact with them.</span></span>

<span data-ttu-id="71b21-118">当提示客户输入来自 bot 的响应时，客户可以在其所选内容对应的小键盘上按某个键。</span><span class="sxs-lookup"><span data-stu-id="71b21-118">When a customer is prompted for a response from the bot, the customer can press a key on their keypad that corresponds to their selection.</span></span> <span data-ttu-id="71b21-119">然后，机器人可以从客户处收集拨号音多频率 (DTMF) 。</span><span class="sxs-lookup"><span data-stu-id="71b21-119">The bot can then gather the dial-tone multi-frequency (DTMF) from the customer.</span></span>

<span data-ttu-id="71b21-120">您可以使用云通信 Api 构建以下 bot：</span><span class="sxs-lookup"><span data-stu-id="71b21-120">You can use the cloud communications APIs to build a bot that:</span></span>

- <span data-ttu-id="71b21-121">[应答](/graph/api/call-answer?view=graph-rest-1.0) 来自客户的呼叫。</span><span class="sxs-lookup"><span data-stu-id="71b21-121">[Answers a call](/graph/api/call-answer?view=graph-rest-1.0) from a customer.</span></span>
- <span data-ttu-id="71b21-122">[播放提示](/graph/api/call-playprompt?view=graph-rest-1.0) 通知并提示客户选择的内容。</span><span class="sxs-lookup"><span data-stu-id="71b21-122">[Plays a prompt](/graph/api/call-playprompt?view=graph-rest-1.0) to inform and prompt a customer for a selection.</span></span>
- <span data-ttu-id="71b21-123">[订阅一个语气](/graph/api/call-subscribetotone?view=graph-rest-1.0) ，以便从客户处收集 DTMF。</span><span class="sxs-lookup"><span data-stu-id="71b21-123">[Subscribes to a tone](/graph/api/call-subscribetotone?view=graph-rest-1.0) to gather the DTMF from a customer.</span></span>
- <span data-ttu-id="71b21-124">将[客户转移](/graph/api/call-transfer?view=graph-rest-1.0)到代理。</span><span class="sxs-lookup"><span data-stu-id="71b21-124">[Transfers a customer](/graph/api/call-transfer?view=graph-rest-1.0) to an agent.</span></span>
- <span data-ttu-id="71b21-125">[结束](/graph/api/call-delete?view=graph-rest-1.0) 与客户的通话。</span><span class="sxs-lookup"><span data-stu-id="71b21-125">[Ends a call](/graph/api/call-delete?view=graph-rest-1.0) with a customer.</span></span>

![为呼叫转移提供选项的 bot 的图像](images/communications-ivr-transfer.png)

<span data-ttu-id="71b21-127">若要在客户和你的 bot 之间创建更智能的交互，当客户收到响应提示时，他们将能够直接谈论他们需要帮助的内容。</span><span class="sxs-lookup"><span data-stu-id="71b21-127">To create a more intelligent interaction between your customers and your bot, when a customer is prompted for a response, they will be able to directly speak about what they need help with.</span></span>

<span data-ttu-id="71b21-128">与自然语言处理服务集成意味着可以对客户的语音进行分析以查找其看法。</span><span class="sxs-lookup"><span data-stu-id="71b21-128">Integrating with a natural language processing service means that the customer's speech can be analyzed for its sentiment.</span></span> <span data-ttu-id="71b21-129">然后，bot 可以相应地响应客户的需求。</span><span class="sxs-lookup"><span data-stu-id="71b21-129">The bot can then respond to the customer's need accordingly.</span></span>

><span data-ttu-id="71b21-130">**注意：** 您不能录制或以其他方式保留来自您的应用程序访问的呼叫或会议的媒体内容或从该媒体内容派生的数据。</span><span class="sxs-lookup"><span data-stu-id="71b21-130">**Note:** You may not record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="71b21-131">请确保您符合有关通信的数据保护和机密性的法律和法规。</span><span class="sxs-lookup"><span data-stu-id="71b21-131">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="71b21-132">有关详细信息，请参阅[使用条款](/legal/microsoft-apis/terms-of-use)并咨询法律顾问。</span><span class="sxs-lookup"><span data-stu-id="71b21-132">Please see the [Terms of Use](/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

<span data-ttu-id="71b21-133">您可以使用云通信 Api 构建以下 bot：</span><span class="sxs-lookup"><span data-stu-id="71b21-133">You can use the cloud communications APIs to build a bot that:</span></span>

- <span data-ttu-id="71b21-134">[应答](/graph/api/call-answer?view=graph-rest-1.0) 来自客户的呼叫。</span><span class="sxs-lookup"><span data-stu-id="71b21-134">[Answers a call](/graph/api/call-answer?view=graph-rest-1.0) from a customer.</span></span>
- <span data-ttu-id="71b21-135">[播放提示](/graph/api/call-playprompt?view=graph-rest-1.0) 以通知并提示客户讲话。</span><span class="sxs-lookup"><span data-stu-id="71b21-135">[Plays a prompt](/graph/api/call-playprompt?view=graph-rest-1.0) to inform and prompt the customer to speak.</span></span>
- <span data-ttu-id="71b21-136">记录客户讲话的[简短音频剪辑](/graph/api/call-record?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="71b21-136">[Records a short audio clip](/graph/api/call-record?view=graph-rest-1.0) of a customer speaking.</span></span>
- <span data-ttu-id="71b21-137">在分析语音后，会向客户发出[提示](/graph/api/call-playprompt?view=graph-rest-1.0)，并提供相应的响应。</span><span class="sxs-lookup"><span data-stu-id="71b21-137">[Plays a prompt](/graph/api/call-playprompt?view=graph-rest-1.0) with the appropriate response to the customer, after their speech is analyzed.</span></span>

![提示用户提供语音响应的 bot 的图像](images/communications-ivr.PNG)

### <a name="collaborate-through-group-calls"></a><span data-ttu-id="71b21-139">通过组调用进行协作</span><span class="sxs-lookup"><span data-stu-id="71b21-139">Collaborate through group calls</span></span>
<span data-ttu-id="71b21-140">允许用户通过创建组呼叫来与同事或客户接洽，以便每个人都可以参与对话。</span><span class="sxs-lookup"><span data-stu-id="71b21-140">Enable users to engage with coworkers or customers by creating a group call so that everyone can contribute to the conversation.</span></span>

<span data-ttu-id="71b21-141">您可以使用云通信 Api 构建以下 bot：</span><span class="sxs-lookup"><span data-stu-id="71b21-141">You can use the cloud communications APIs to build a bot that:</span></span>

- <span data-ttu-id="71b21-142">创建具有多个参与者[的组呼叫](/graph/api/application-post-calls?view=graph-rest-1.0#example-3-create-a-group-call-with-service-hosted-media)。</span><span class="sxs-lookup"><span data-stu-id="71b21-142">[Creates a group call](/graph/api/application-post-calls?view=graph-rest-1.0#example-3-create-a-group-call-with-service-hosted-media) with multiple participants.</span></span>
- <span data-ttu-id="71b21-143">[邀请另一个 bot 或用户](/graph/api/participant-invite?view=graph-rest-1.0) 到现有的组呼叫。</span><span class="sxs-lookup"><span data-stu-id="71b21-143">[Invites another bot or user](/graph/api/participant-invite?view=graph-rest-1.0) to an existing group call.</span></span>
- <span data-ttu-id="71b21-144">将[现有的组呼叫](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media)作为 bot 加入。</span><span class="sxs-lookup"><span data-stu-id="71b21-144">[Joins an existing group call](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media) as a bot.</span></span>
- <span data-ttu-id="71b21-145">列出组呼叫中[的参与者](/graph/api/call-list-participants?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="71b21-145">[Lists the participants](/graph/api/call-list-participants?view=graph-rest-1.0) in the group call.</span></span>
- <span data-ttu-id="71b21-146">[Mutes 其他参与者](/graph/api/participant-mute?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="71b21-146">[Mutes another participant](/graph/api/participant-mute?view=graph-rest-1.0).</span></span>

### <a name="send-reminders-reliably"></a><span data-ttu-id="71b21-147">可靠地发送提醒</span><span class="sxs-lookup"><span data-stu-id="71b21-147">Send reminders reliably</span></span>
<span data-ttu-id="71b21-148">若要使用户能够向客户发送约会提醒或付款截止日期的提醒，可以让 bot 自动呼叫客户。</span><span class="sxs-lookup"><span data-stu-id="71b21-148">To enable users to send customers a reminder for an appointment or a reminder for a payment deadline that’s approaching, you can have a bot call the customer automatically.</span></span> <!--If the customer misses the call, it will leave a voicemail with the automated message. (Add this back once bot to PSTN calling works)-->

<span data-ttu-id="71b21-149">您可以使用云通信 Api 构建以下 bot：</span><span class="sxs-lookup"><span data-stu-id="71b21-149">You can use the cloud communications APIs to build a bot that:</span></span>

- <span data-ttu-id="71b21-150">在团队中[打电话给客户](/graph/api/application-post-calls?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="71b21-150">[Calls a customer](/graph/api/application-post-calls?view=graph-rest-1.0) on Teams.</span></span>
- <span data-ttu-id="71b21-151">[播放录制的提示](/graph/api/call-playprompt?view=graph-rest-1.0) 以充当提醒。</span><span class="sxs-lookup"><span data-stu-id="71b21-151">[Plays a recorded prompt](/graph/api/call-playprompt?view=graph-rest-1.0) to serve as a reminder.</span></span>
- <span data-ttu-id="71b21-152">[结束呼叫](/graph/api/call-delete?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="71b21-152">[Ends the call](/graph/api/call-delete?view=graph-rest-1.0).</span></span>


### <a name="set-up-online-meetings"></a><span data-ttu-id="71b21-153">设置联机会议</span><span class="sxs-lookup"><span data-stu-id="71b21-153">Set up online meetings</span></span>
<span data-ttu-id="71b21-154">无论是在医生与患者之间还是在用户与其直接下属之间安排会议，您可以生成可生成用户可以依赖的会议的解决方案。</span><span class="sxs-lookup"><span data-stu-id="71b21-154">Whether scheduling a meeting between a doctor and a patient or between a user and their direct reports, you can build solutions that generate meetings that users can rely on.</span></span> <span data-ttu-id="71b21-155">为提高灵活性，用户可以呼叫其他用户，并在正在进行会议时邀请他们加入会议。</span><span class="sxs-lookup"><span data-stu-id="71b21-155">For added flexibility, users can call other users and invite them to the meeting while it's ongoing.</span></span>

<span data-ttu-id="71b21-156">您可以使用云通信 Api 执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="71b21-156">You can use the cloud communications APIs to:</span></span>

- <span data-ttu-id="71b21-157">让用户 [创建联机会议](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="71b21-157">Have a user [create an online meeting](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="71b21-158">让用户检索联机会议的 [详细信息](/graph/api/onlinemeeting-get?view=graph-rest-1.0) 。</span><span class="sxs-lookup"><span data-stu-id="71b21-158">Have a user [retrieve the details](/graph/api/onlinemeeting-get?view=graph-rest-1.0) of an online meeting.</span></span>
- <span data-ttu-id="71b21-159">拥有机器人或用户 [加入联机会议](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media)。</span><span class="sxs-lookup"><span data-stu-id="71b21-159">Have a bot or a user [join an online meeting](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media).</span></span>

## <a name="api-reference"></a><span data-ttu-id="71b21-160">API 参考</span><span class="sxs-lookup"><span data-stu-id="71b21-160">API reference</span></span>
<span data-ttu-id="71b21-161">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="71b21-161">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="71b21-162">Microsoft Graph 中的云通信 Api (v1.0) </span><span class="sxs-lookup"><span data-stu-id="71b21-162">Cloud Communications APIs in Microsoft Graph (v1.0)</span></span>](/graph/api/resources/communications-api-overview?view=graph-rest-1.0)
- [<span data-ttu-id="71b21-163">Microsoft Graph 中的云通信 Api (beta) </span><span class="sxs-lookup"><span data-stu-id="71b21-163">Cloud Communications APIs in Microsoft Graph (beta)</span></span>](/graph/api/resources/communications-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="71b21-164">后续步骤</span><span class="sxs-lookup"><span data-stu-id="71b21-164">Next steps</span></span>

- <span data-ttu-id="71b21-165">使用 bot [开始](cloud-communications-get-started.md)。</span><span class="sxs-lookup"><span data-stu-id="71b21-165">Use bots to [get started](cloud-communications-get-started.md).</span></span>
- <span data-ttu-id="71b21-166">了解有关 [呼叫](cloud-communications-calls.md)、 [媒体](cloud-communications-media.md)和 [联机会议](cloud-communications-online-meetings.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="71b21-166">Learn more about [calls](cloud-communications-calls.md), [media](cloud-communications-media.md), and [online meetings](cloud-communications-online-meetings.md).</span></span>
- <span data-ttu-id="71b21-167">查看 API 使用 [限制](throttling.md#cloud-communication-service-limits)。</span><span class="sxs-lookup"><span data-stu-id="71b21-167">View the API usage [limits](throttling.md#cloud-communication-service-limits).</span></span>
- <span data-ttu-id="71b21-168">了解如何管理你的 bot 的 [电话号码](cloud-communications-phone-number.md) 。</span><span class="sxs-lookup"><span data-stu-id="71b21-168">Learn how to [manage phone numbers](cloud-communications-phone-number.md) for your bots.</span></span>

## <a name="see-also"></a><span data-ttu-id="71b21-169">另请参阅</span><span class="sxs-lookup"><span data-stu-id="71b21-169">See also</span></span>

- [<span data-ttu-id="71b21-170">委派和应用程序权限</span><span class="sxs-lookup"><span data-stu-id="71b21-170">Delegated and application permissions</span></span>](/azure/active-directory/develop/v1-permissions-and-consent)
- [<span data-ttu-id="71b21-171">通话权限</span><span class="sxs-lookup"><span data-stu-id="71b21-171">Calls permissions</span></span>](./permissions-reference.md#calls-permissions)
- [<span data-ttu-id="71b21-172">联机会议权限</span><span class="sxs-lookup"><span data-stu-id="71b21-172">Online meeting permissions</span></span>](./permissions-reference.md#online-meetings-permissions)
- [<span data-ttu-id="71b21-173">云通信示例</span><span class="sxs-lookup"><span data-stu-id="71b21-173">Cloud communications samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples)