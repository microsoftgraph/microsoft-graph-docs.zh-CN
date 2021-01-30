---
title: 云通信 API 概述
description: Microsoft Graph 中的云通信 API 为应用和服务通过各种通信相关功能（如通话和联机会议）与用户交互的方式添加了一个新维度。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 572ce19e14779615ac8db514101df7d944b1d819
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059593"
---
# <a name="cloud-communications-api-overview"></a><span data-ttu-id="25f1f-103">云通信 API 概述</span><span class="sxs-lookup"><span data-stu-id="25f1f-103">Cloud communications API overview</span></span>
<span data-ttu-id="25f1f-104">Microsoft Graph 中的云通信 API 为应用和服务通过各种通信相关功能（如通话和联机会议）与用户交互的方式添加了一个新维度。</span><span class="sxs-lookup"><span data-stu-id="25f1f-104">The cloud communications APIs in Microsoft Graph add a new dimension to how your apps and services interact with users through various communications related features, such as calling and online meetings.</span></span> <span data-ttu-id="25f1f-105">通过了解如何响应客户的需求以及员工如何相互协作来发展你的业务。</span><span class="sxs-lookup"><span data-stu-id="25f1f-105">Grow your business by expediting how you respond to your customers’ needs and how your employees collaborate with each other.</span></span>

## <a name="why-integrate-with-the-cloud-communications-apis"></a><span data-ttu-id="25f1f-106">为什么与云通信 API 集成？</span><span class="sxs-lookup"><span data-stu-id="25f1f-106">Why integrate with the cloud communications APIs?</span></span>

<span data-ttu-id="25f1f-107">发现使用云通信 API 构建服务应用程序的好处， ([自动程序](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html?q=create%20bot)) 。</span><span class="sxs-lookup"><span data-stu-id="25f1f-107">Discover the benefits of using cloud communications APIs to build service applications ([bots](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html?q=create%20bot)).</span></span>

### <a name="handle-incoming-calls"></a><span data-ttu-id="25f1f-108">处理传入呼叫</span><span class="sxs-lookup"><span data-stu-id="25f1f-108">Handle incoming calls</span></span>

<span data-ttu-id="25f1f-109">当工作人员收到大量业务呼叫，并且无法或无法高效应答所有呼叫时，情况可能会很不知所措。</span><span class="sxs-lookup"><span data-stu-id="25f1f-109">It can be overwhelming at times when workers receive a lot of business calls and it isn't possible, or productive, to answer all of them.</span></span> <span data-ttu-id="25f1f-110">机器人可以充当前台助理并处理这些呼叫，具体方法为拒绝看起来像垃圾邮件呼叫 (将) 呼叫重定向到其他号码。</span><span class="sxs-lookup"><span data-stu-id="25f1f-110">A bot can serve as a front-desk assistant and handle these calls by rejecting what seem like spam calls, and redirecting (forwarding) specific calls to a different number.</span></span>

<span data-ttu-id="25f1f-111">您可以使用云通信 API：</span><span class="sxs-lookup"><span data-stu-id="25f1f-111">You can use the cloud communications APIs to:</span></span>

- <span data-ttu-id="25f1f-112">让用户通过 VoIP [呼叫](/graph/api/application-post-calls?view=graph-rest-1.0) 机器人。</span><span class="sxs-lookup"><span data-stu-id="25f1f-112">Have a user [call a bot](/graph/api/application-post-calls?view=graph-rest-1.0) through VoIP.</span></span>
- <span data-ttu-id="25f1f-113">如有必要， [让机器人将传入呼叫](/graph/api/call-redirect?view=graph-rest-1.0) 重定向到相应的代理。</span><span class="sxs-lookup"><span data-stu-id="25f1f-113">Have a bot [redirect the incoming call](/graph/api/call-redirect?view=graph-rest-1.0) to the appropriate agent if necessary.</span></span>
- <span data-ttu-id="25f1f-114">拥有自动程序[应答](/graph/api/call-answer?view=graph-rest-1.0)[或拒绝](/graph/api/call-reject?view=graph-rest-1.0)呼叫。</span><span class="sxs-lookup"><span data-stu-id="25f1f-114">Have a bot [answer](/graph/api/call-answer?view=graph-rest-1.0) or [reject](/graph/api/call-reject?view=graph-rest-1.0) the call.</span></span>


### <a name="simplify-the-customer-service-experience"></a><span data-ttu-id="25f1f-115">简化客户服务体验</span><span class="sxs-lookup"><span data-stu-id="25f1f-115">Simplify the customer service experience</span></span>
<span data-ttu-id="25f1f-116">无论你拥有大型支持人员服务还是小型店面，都很难处理多个客户请求，尤其是在你事先没有关于他们尝试解决的问题的上下文时。</span><span class="sxs-lookup"><span data-stu-id="25f1f-116">Whether you own a large helpdesk service or a small storefront, it can be difficult to handle multiple customer requests, especially if you don’t have any context of what problem they’re trying to solve beforehand.</span></span> <span data-ttu-id="25f1f-117">通过 IVR (互动语音响应) 处理来自客户的传入呼叫，机器人最初将与之交互。</span><span class="sxs-lookup"><span data-stu-id="25f1f-117">Handle incoming calls from customers through an **Interactive Voice Response** (IVR) system, where a bot will initially interact with them.</span></span>

<span data-ttu-id="25f1f-118">当提示客户从自动程序响应时，客户可以按键盘上与其选择对应的键。</span><span class="sxs-lookup"><span data-stu-id="25f1f-118">When a customer is prompted for a response from the bot, the customer can press a key on their keypad that corresponds to their selection.</span></span> <span data-ttu-id="25f1f-119">然后，机器人可以收集来自客户的 DTMF (多) 拨号音。</span><span class="sxs-lookup"><span data-stu-id="25f1f-119">The bot can then gather the dial-tone multi-frequency (DTMF) from the customer.</span></span>

<span data-ttu-id="25f1f-120">可以使用云通信 API 生成以下机器人：</span><span class="sxs-lookup"><span data-stu-id="25f1f-120">You can use the cloud communications APIs to build a bot that:</span></span>

- <span data-ttu-id="25f1f-121">[应答来自](/graph/api/call-answer?view=graph-rest-1.0) 客户的呼叫。</span><span class="sxs-lookup"><span data-stu-id="25f1f-121">[Answers a call](/graph/api/call-answer?view=graph-rest-1.0) from a customer.</span></span>
- <span data-ttu-id="25f1f-122">[播放提示](/graph/api/call-playprompt?view=graph-rest-1.0) 以通知和提示客户进行选择。</span><span class="sxs-lookup"><span data-stu-id="25f1f-122">[Plays a prompt](/graph/api/call-playprompt?view=graph-rest-1.0) to inform and prompt a customer for a selection.</span></span>
- <span data-ttu-id="25f1f-123">[订阅从客户收集](/graph/api/call-subscribetotone?view=graph-rest-1.0) DTMF 的音调。</span><span class="sxs-lookup"><span data-stu-id="25f1f-123">[Subscribes to a tone](/graph/api/call-subscribetotone?view=graph-rest-1.0) to gather the DTMF from a customer.</span></span>
- <span data-ttu-id="25f1f-124">[将客户转移到](/graph/api/call-transfer?view=graph-rest-1.0) 代理。</span><span class="sxs-lookup"><span data-stu-id="25f1f-124">[Transfers a customer](/graph/api/call-transfer?view=graph-rest-1.0) to an agent.</span></span>
- <span data-ttu-id="25f1f-125">[结束与客户](/graph/api/call-delete?view=graph-rest-1.0) 的通话。</span><span class="sxs-lookup"><span data-stu-id="25f1f-125">[Ends a call](/graph/api/call-delete?view=graph-rest-1.0) with a customer.</span></span>

![提供呼叫转移选项的机器人的图像](images/communications-ivr-transfer.png)

<span data-ttu-id="25f1f-127">为了在您的客户和机器人之间创建更智能的交互，当系统提示客户做出响应时，他们将能够直接说出他们需要帮助的方面。</span><span class="sxs-lookup"><span data-stu-id="25f1f-127">To create a more intelligent interaction between your customers and your bot, when a customer is prompted for a response, they will be able to directly speak about what they need help with.</span></span>

<span data-ttu-id="25f1f-128">与自然语言处理服务集成意味着可以分析客户的语音，了解其观点。</span><span class="sxs-lookup"><span data-stu-id="25f1f-128">Integrating with a natural language processing service means that the customer's speech can be analyzed for its sentiment.</span></span> <span data-ttu-id="25f1f-129">然后，机器人可以相应地响应客户的需要。</span><span class="sxs-lookup"><span data-stu-id="25f1f-129">The bot can then respond to the customer's need accordingly.</span></span>

><span data-ttu-id="25f1f-130">**注意：** You may not record or otherwise persist media content from calls or meetings that your application accesses， or data derived from that media content.</span><span class="sxs-lookup"><span data-stu-id="25f1f-130">**Note:** You may not record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="25f1f-131">确保遵守有关通信数据保护和机密性的领域的法律和法规。</span><span class="sxs-lookup"><span data-stu-id="25f1f-131">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="25f1f-132">有关详细信息，请参阅[使用条款](/legal/microsoft-apis/terms-of-use)并咨询法律顾问。</span><span class="sxs-lookup"><span data-stu-id="25f1f-132">Please see the [Terms of Use](/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

<span data-ttu-id="25f1f-133">可以使用云通信 API 生成以下机器人：</span><span class="sxs-lookup"><span data-stu-id="25f1f-133">You can use the cloud communications APIs to build a bot that:</span></span>

- <span data-ttu-id="25f1f-134">[应答来自](/graph/api/call-answer?view=graph-rest-1.0) 客户的呼叫。</span><span class="sxs-lookup"><span data-stu-id="25f1f-134">[Answers a call](/graph/api/call-answer?view=graph-rest-1.0) from a customer.</span></span>
- <span data-ttu-id="25f1f-135">[播放提示](/graph/api/call-playprompt?view=graph-rest-1.0) 以通知并提示客户说话。</span><span class="sxs-lookup"><span data-stu-id="25f1f-135">[Plays a prompt](/graph/api/call-playprompt?view=graph-rest-1.0) to inform and prompt the customer to speak.</span></span>
- <span data-ttu-id="25f1f-136">[录制客户说话的](/graph/api/call-record?view=graph-rest-1.0) 简短音频剪辑。</span><span class="sxs-lookup"><span data-stu-id="25f1f-136">[Records a short audio clip](/graph/api/call-record?view=graph-rest-1.0) of a customer speaking.</span></span>
- <span data-ttu-id="25f1f-137">[在分析客户的](/graph/api/call-playprompt?view=graph-rest-1.0) 语音后，向客户播放相应响应的提示。</span><span class="sxs-lookup"><span data-stu-id="25f1f-137">[Plays a prompt](/graph/api/call-playprompt?view=graph-rest-1.0) with the appropriate response to the customer, after their speech is analyzed.</span></span>

![提示用户提供语音响应的自动程序的图像](images/communications-ivr.PNG)

### <a name="collaborate-through-group-calls"></a><span data-ttu-id="25f1f-139">通过组通话进行协作</span><span class="sxs-lookup"><span data-stu-id="25f1f-139">Collaborate through group calls</span></span>
<span data-ttu-id="25f1f-140">允许用户通过创建群组通话与同事或客户互动，以便每个人都可以参与对话。</span><span class="sxs-lookup"><span data-stu-id="25f1f-140">Enable users to engage with coworkers or customers by creating a group call so that everyone can contribute to the conversation.</span></span>

<span data-ttu-id="25f1f-141">可以使用云通信 API 生成以下机器人：</span><span class="sxs-lookup"><span data-stu-id="25f1f-141">You can use the cloud communications APIs to build a bot that:</span></span>

- <span data-ttu-id="25f1f-142">[创建包含多个参与者的](/graph/api/application-post-calls?view=graph-rest-1.0#example-3-create-a-group-call-with-service-hosted-media) 组呼叫。</span><span class="sxs-lookup"><span data-stu-id="25f1f-142">[Creates a group call](/graph/api/application-post-calls?view=graph-rest-1.0#example-3-create-a-group-call-with-service-hosted-media) with multiple participants.</span></span>
- <span data-ttu-id="25f1f-143">[邀请其他机器人或用户](/graph/api/participant-invite?view=graph-rest-1.0) 加入现有组通话。</span><span class="sxs-lookup"><span data-stu-id="25f1f-143">[Invites another bot or user](/graph/api/participant-invite?view=graph-rest-1.0) to an existing group call.</span></span>
- <span data-ttu-id="25f1f-144">[以机器人方式加入](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media) 现有组呼叫。</span><span class="sxs-lookup"><span data-stu-id="25f1f-144">[Joins an existing group call](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media) as a bot.</span></span>
- <span data-ttu-id="25f1f-145">[列出组](/graph/api/call-list-participants?view=graph-rest-1.0) 通话中的参与者。</span><span class="sxs-lookup"><span data-stu-id="25f1f-145">[Lists the participants](/graph/api/call-list-participants?view=graph-rest-1.0) in the group call.</span></span>
- <span data-ttu-id="25f1f-146">[将另一个参与者静音](/graph/api/participant-mute?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="25f1f-146">[Mutes another participant](/graph/api/participant-mute?view=graph-rest-1.0).</span></span>

### <a name="send-reminders-reliably"></a><span data-ttu-id="25f1f-147">可靠地发送提醒</span><span class="sxs-lookup"><span data-stu-id="25f1f-147">Send reminders reliably</span></span>
<span data-ttu-id="25f1f-148">若要使用户能够为客户发送约会提醒或接近付款截止时间提醒，你可以让机器人自动呼叫客户。</span><span class="sxs-lookup"><span data-stu-id="25f1f-148">To enable users to send customers a reminder for an appointment or a reminder for a payment deadline that’s approaching, you can have a bot call the customer automatically.</span></span> <!--If the customer misses the call, it will leave a voicemail with the automated message. (Add this back once bot to PSTN calling works)-->

<span data-ttu-id="25f1f-149">可以使用云通信 API 生成以下机器人：</span><span class="sxs-lookup"><span data-stu-id="25f1f-149">You can use the cloud communications APIs to build a bot that:</span></span>

- <span data-ttu-id="25f1f-150">[在](/graph/api/application-post-calls?view=graph-rest-1.0) Teams 上呼叫客户。</span><span class="sxs-lookup"><span data-stu-id="25f1f-150">[Calls a customer](/graph/api/application-post-calls?view=graph-rest-1.0) on Teams.</span></span>
- <span data-ttu-id="25f1f-151">[播放录制的提示](/graph/api/call-playprompt?view=graph-rest-1.0) 以用作提醒。</span><span class="sxs-lookup"><span data-stu-id="25f1f-151">[Plays a recorded prompt](/graph/api/call-playprompt?view=graph-rest-1.0) to serve as a reminder.</span></span>
- <span data-ttu-id="25f1f-152">[结束调用](/graph/api/call-delete?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="25f1f-152">[Ends the call](/graph/api/call-delete?view=graph-rest-1.0).</span></span>


### <a name="set-up-online-meetings"></a><span data-ttu-id="25f1f-153">设置联机会议</span><span class="sxs-lookup"><span data-stu-id="25f1f-153">Set up online meetings</span></span>
<span data-ttu-id="25f1f-154">无论是安排患者与患者之间的会议，还是安排用户及其直接下属之间的会议，都可以生成生成用户可依赖的会议的解决方案。</span><span class="sxs-lookup"><span data-stu-id="25f1f-154">Whether scheduling a meeting between a doctor and a patient or between a user and their direct reports, you can build solutions that generate meetings that users can rely on.</span></span> <span data-ttu-id="25f1f-155">为了增加灵活性，用户可以呼叫其他用户，并邀请他们在会议进行期间参加会议。</span><span class="sxs-lookup"><span data-stu-id="25f1f-155">For added flexibility, users can call other users and invite them to the meeting while it's ongoing.</span></span>

<span data-ttu-id="25f1f-156">您可以使用云通信 API：</span><span class="sxs-lookup"><span data-stu-id="25f1f-156">You can use the cloud communications APIs to:</span></span>

- <span data-ttu-id="25f1f-157">让用户创建 [联机会议](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="25f1f-157">Have a user [create an online meeting](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="25f1f-158">让用户 [检索联机](/graph/api/onlinemeeting-get?view=graph-rest-1.0) 会议的详细信息。</span><span class="sxs-lookup"><span data-stu-id="25f1f-158">Have a user [retrieve the details](/graph/api/onlinemeeting-get?view=graph-rest-1.0) of an online meeting.</span></span>
- <span data-ttu-id="25f1f-159">使机器人或用户 [加入联机会议](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media)。</span><span class="sxs-lookup"><span data-stu-id="25f1f-159">Have a bot or a user [join an online meeting](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media).</span></span>

## <a name="api-reference"></a><span data-ttu-id="25f1f-160">API 参考</span><span class="sxs-lookup"><span data-stu-id="25f1f-160">API reference</span></span>
<span data-ttu-id="25f1f-161">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="25f1f-161">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="25f1f-162">Microsoft Graph 中的云通信 API (v1.0) </span><span class="sxs-lookup"><span data-stu-id="25f1f-162">Cloud Communications APIs in Microsoft Graph (v1.0)</span></span>](/graph/api/resources/communications-api-overview?view=graph-rest-1.0)
- [<span data-ttu-id="25f1f-163">Microsoft Graph (beta) 中的云通信 API </span><span class="sxs-lookup"><span data-stu-id="25f1f-163">Cloud Communications APIs in Microsoft Graph (beta)</span></span>](/graph/api/resources/communications-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="25f1f-164">后续步骤</span><span class="sxs-lookup"><span data-stu-id="25f1f-164">Next steps</span></span>

- <span data-ttu-id="25f1f-165">使用机器人[开始。](cloud-communications-get-started.md)</span><span class="sxs-lookup"><span data-stu-id="25f1f-165">Use bots to [get started](cloud-communications-get-started.md).</span></span>
- <span data-ttu-id="25f1f-166">了解有关[呼叫、](cloud-communications-calls.md)[媒体和](cloud-communications-media.md)联机[会议有关详细信息](cloud-communications-online-meetings.md)。</span><span class="sxs-lookup"><span data-stu-id="25f1f-166">Learn more about [calls](cloud-communications-calls.md), [media](cloud-communications-media.md), and [online meetings](cloud-communications-online-meetings.md).</span></span>
- <span data-ttu-id="25f1f-167">查看 API 使用 [限制](throttling.md#cloud-communication-service-limits)。</span><span class="sxs-lookup"><span data-stu-id="25f1f-167">View the API usage [limits](throttling.md#cloud-communication-service-limits).</span></span>
- <span data-ttu-id="25f1f-168">了解如何 [管理机器人](cloud-communications-phone-number.md) 的电话号码。</span><span class="sxs-lookup"><span data-stu-id="25f1f-168">Learn how to [manage phone numbers](cloud-communications-phone-number.md) for your bots.</span></span>

## <a name="see-also"></a><span data-ttu-id="25f1f-169">另请参阅</span><span class="sxs-lookup"><span data-stu-id="25f1f-169">See also</span></span>

- [<span data-ttu-id="25f1f-170">委派和应用程序权限</span><span class="sxs-lookup"><span data-stu-id="25f1f-170">Delegated and application permissions</span></span>](/azure/active-directory/develop/v1-permissions-and-consent)
- [<span data-ttu-id="25f1f-171">通话权限</span><span class="sxs-lookup"><span data-stu-id="25f1f-171">Calls permissions</span></span>](./permissions-reference.md#calls-permissions)
- [<span data-ttu-id="25f1f-172">联机会议权限</span><span class="sxs-lookup"><span data-stu-id="25f1f-172">Online meeting permissions</span></span>](./permissions-reference.md#online-meetings-permissions)
- [<span data-ttu-id="25f1f-173">云通信示例</span><span class="sxs-lookup"><span data-stu-id="25f1f-173">Cloud communications samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples)
