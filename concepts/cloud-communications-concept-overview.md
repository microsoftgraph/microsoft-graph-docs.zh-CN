---
title: 云通信 API 概述
description: 使用 Microsoft Graph 中的云通信 API 生成机器人来处理传入呼叫、通过组调用进行协作、发送提醒和设置会议。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: 8ab2494a86abb1298cc4a6cb4fe1172b8374643d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436361"
---
# <a name="cloud-communications-api-overview"></a>云通信 API 概述

Microsoft Graph 中的云通信 API 为应用和服务如何通过各种与通信相关的功能（例如通话和联机会议）与用户交互添加了一个新维度。 通过加快响应客户需求的方式以及员工相互协作的方式来发展业务。

若要发现使用云通信 API ([机器人](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html?q=create%20bot)) 生成服务应用程序的好处，请参阅以下部分。

## <a name="handle-incoming-calls"></a>处理传入调用

当工人接到很多商业电话，而不能或没有生产力地回答所有这些电话时，这可能会让人难以忍受。 机器人可以充当前台助理，并通过拒绝类似垃圾邮件的呼叫来处理这些呼叫，并将 () 特定调用重定向到其他号码。

可以使用云通信 API 执行以下操作：

- 让用户通过 VoIP [调用机器人](/graph/api/application-post-calls) 。
- 如有必要，让机器人 [将传入调用重定](/graph/api/call-redirect) 向到相应的代理。
- 有一个机器人 [应答](/graph/api/call-answer) 或 [拒绝](/graph/api/call-reject) 呼叫。


## <a name="simplify-the-customer-service-experience"></a>简化客户服务体验

无论你拥有大型支持服务还是小型店面，都可能很难处理多个客户请求，尤其是如果你没有任何关于他们事先尝试解决的问题的任何上下文。 通过 **交互式语音响应** (IVR) 系统处理来自客户的传入呼叫，机器人最初将在其中与他们交互。

当系统提示客户从机器人发出响应时，客户可以在其键盘上按一个与所选内容相对应的密钥。 然后，机器人可以从客户收集 DTMF)  (拨号多频率。

可以使用云通信 API 生成以下功能的机器人：

- [接听客户打来的电话](/graph/api/call-answer) 。
- [播放提示](/graph/api/call-playprompt) 以通知客户并提示客户进行选择。
- [订阅语气](/graph/api/call-subscribetotone) 以从客户处收集 DTMF。
- [将客户传输](/graph/api/call-transfer) 到代理。
- 结束与客户[的通话](/graph/api/call-delete)。

![提供呼叫传输选项的机器人的图像](images/communications-ivr-transfer.png)

若要在客户和机器人之间创建更智能的交互，当客户收到响应提示时，他们将能够直接谈论他们需要的帮助。

与自然语言处理服务集成意味着客户的语音可以分析其情绪。 然后，机器人可以相应地响应客户的需求。

> [!NOTE]
> 不得记录或保存来自应用程序访问的呼叫或会议的媒体内容，也不得保留从该媒体内容派生的数据。 确保遵守有关数据保护和通信保密性的相关法律和法规。 有关详细信息，请参阅[使用条款](/legal/microsoft-apis/terms-of-use)并咨询法律顾问。

可以使用云通信 API 生成以下功能的机器人：

- [接听客户打来的电话](/graph/api/call-answer) 。
- [播放提示](/graph/api/call-playprompt) 以通知并提示客户发言。
- 记录客户讲话的[简短音频剪辑](/graph/api/call-record)。
- [在](/graph/api/call-playprompt) 分析客户的语音后，使用相应的响应播放提示。

![提示用户发出语音响应的机器人的图像](images/communications-ivr.PNG)

## <a name="collaborate-through-group-calls"></a>通过组调用进行协作
通过创建组呼叫，使用户能够与同事或客户互动，以便每个人都可以参与对话。

可以使用云通信 API 生成以下功能的机器人：

- [创建具有多个参与者的组调用](/graph/api/application-post-calls#example-3-create-a-group-call-with-service-hosted-media) 。
- [邀请其他机器人或用户](/graph/api/participant-invite) 进行现有组调用。
- 以机器人身份[加入现有组调用](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media)。
- [列出](/graph/api/call-list-participants) 组调用中的参与者。
- [将另一个参与者静音](/graph/api/participant-mute)。

## <a name="send-reminders-reliably"></a>可靠地发送提醒
若要使用户能够向客户发送约会提醒或付款截止时间即将到来的提醒，可以让机器人自动调用客户。 <!--If the customer misses the call, it will leave a voicemail with the automated message. (Add this back once bot to PSTN calling works)-->

可以使用云通信 API 生成以下功能的机器人：

- 在 Teams 上[调用客户](/graph/api/application-post-calls)。
- [播放记录的提示](/graph/api/call-playprompt) 以用作提醒。
- [结束调用](/graph/api/call-delete)。


## <a name="set-up-online-meetings"></a>设置联机会议
无论是安排医生和病人之间的会议，还是在用户与其直接报告之间安排会议，都可以生成生成用户可以依赖的会议的解决方案。 为了增加灵活性，用户可以调用其他用户，并在会议进行期间邀请他们参加会议。

可以使用云通信 API 执行以下操作：

- 让用户 [创建联机会议](/graph/api/application-post-onlinemeetings)。
- 让用户检索联机会议的 [详细信息](/graph/api/onlinemeeting-get) 。
- 让机器人或用户 [加入联机会议](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media)。

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

- [Microsoft Graph v1.0 中的云通信 API](/graph/api/resources/communications-api-overview?view=graph-rest-1.0&preserve-view=true)
- [Microsoft Graph beta 中的云通信 API](/graph/api/resources/communications-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>后续步骤

- 使用机器人 [入门](cloud-communications-get-started.md)。
- 详细了解 [呼叫](cloud-communications-calls.md)、 [媒体](cloud-communications-media.md)和 [在线会议](cloud-communications-online-meetings.md)。
- 查看 API 使用 [限制](throttling.md#cloud-communication-service-limits)。
- 了解如何管理机器人的 [电话号码](cloud-communications-phone-number.md) 。

## <a name="see-also"></a>另请参阅

- [委派权限和应用程序权限](/azure/active-directory/develop/v1-permissions-and-consent)
- [通话权限](./permissions-reference.md#calls-permissions)
- [联机会议权限](./permissions-reference.md#online-meetings-permissions)
- [云通信 API 示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples)
