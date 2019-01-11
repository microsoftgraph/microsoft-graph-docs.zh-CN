---
title: 使用呼叫和 Microsoft Graph 中的联机会议 API
description: Microsoft Graph 呼叫和联机会议 API 将新的维度添加到您的应用程序和服务的交互方式与用户通过启用语音和视频功能。 API，您可以创建呼叫和接收来自用户和应用程序中的 Microsoft 团队的呼叫。 这些 Api 可用于构建可以充当呼叫或会议中的参与者的服务应用程序 （自动程序）。
author: VinodRavichandran
localization_priority: Priority
ms.openlocfilehash: d7912f587dcc0181a2edd4072f0e07aa643d66be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876529"
---
# <a name="working-with-the-calls-and-online-meetings-api-in-microsoft-graph"></a>使用呼叫和 Microsoft Graph 中的联机会议 API

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

Microsoft Graph 呼叫和联机会议 API 将新的维度添加到您的应用程序和服务的交互方式与用户通过启用语音和视频功能。 API，您可以创建呼叫和接收来自用户和应用程序中的 Microsoft 团队的呼叫。 这些 Api 可用于构建可以充当呼叫或会议中的参与者的服务应用程序 （自动程序）。

## <a name="call-types"></a>呼叫类型

呼叫被分类为对等或多方呼叫。 用户可以启动与您自动程序的对等呼叫或邀请您自动程序到现有多方会议。 用户正在邀请到对等呼叫自动程序时，不不需要任何权限。 参与多方呼叫您 bot、 bot 需要具有加入的组呼叫由租户管理员权限。

![显示对等和多方呼叫图像](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/call-types.png)

如果您自动程序创建呼叫，它需要用启动或启动组呼叫权限。 您自动程序已创建的对等呼叫或多方呼叫的选项。

- 对等呼叫，需要指定唯一的目标和没有会议坐标 bot。 
- 如果您 bot 发起呼叫与多个参与者，在后台设置为临时会议和所有人加入会议。 如果指定会议坐标，那么即使只有一个目标多方呼叫是可以设置。

可能对等以启动并升级到多方呼叫。 会议已自动设置和媒体重定向到会议。 提供您自动程序已启动组呼叫权限，您自动程序可以通过邀请其他人，启动升级。 如果升级启动另一个参与者，并且 bot 没有加入组呼叫权限，则从调用丢弃您自动程序。

> **重要：** 当从对等情况下，呼叫上报给多方时，并非所有的多方功能均可用。 具体而言，自动程序不会收到名单更新。

## <a name="signaling"></a>信号

### <a name="incoming-call"></a>传入呼叫

若要接收传入呼叫，您需要注册调用 bot。 Bot 接收传入通知时，它具有以下选项。

| 方法                              | 说明                                  |
|:------------------------------------|:---------------------------------------------|
| [答案](../api/call-answer.md)     | 应答传入呼叫。                    |
| [Reject](../api/call-reject.md)     | 拒绝和挂断呼叫。                  |
| [重定向](../api/call-redirect.md) | 将呼叫重定向。                           |

Bot 可以呼叫重定向到另一个用户或自动程序。 Bot 可以还将其重定向到用户的语音邮件。

![显示自动程序重定向至语音邮件的呼叫的图像](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/call-handling.png)

> **重要：** 重定向或发起出站 pstn 呼叫当前不支持。

### <a name="in-call"></a>呼叫中

自动程序的操作是调用对象上可用。 这些呼叫中的参与者作为影响 bot。

| 方法                                                            | 说明                                  |
|:------------------------------------------------------------------|:---------------------------------------------|
| [设置为静音](../api/call-mute.md)                                       | 在呼叫中的静音自我。                       |
| [取消静音](../api/call-unmute.md)                                   | 在呼叫中的取消静音自我。                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | 在名单中的自助更新元数据。          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) | 启动和停止共享的调用中的屏幕。   |

要与其他参与者的呼叫进行交互，使用参与者对象。

| 方法                                                            | 说明                                  |
|:------------------------------------------------------------------|:---------------------------------------------|
| [参与者列表](../api/call-list-participants.md)             | 获取参与者对象集合。         |
| [邀请参与者](../api/participant-invite.md)               | 邀请参与者加入活动呼叫。      |
| [将所有参与者设为都静音](../api/participant-muteall.md)            | 将呼叫中的所有参与者设为都静音。           |

## <a name="media"></a>媒体

通过 Microsoft 实时媒体平台管理媒体处理。 实时媒体平台帮助 bot 参与 Microsoft 团队音频/视频呼叫和会议。 它允许实时 bot 参加对等和多方呼叫。

当 bot 应答传入呼叫，或加入新的或现有的呼叫时，则需要告知实时媒体平台将如何处理媒体。 如果您要构建互动语音响应 (IVR) 系统，您可以卸载昂贵音频处理 Microsoft 承载的服务媒体组件。 如果您自动程序需要直接访问媒体流，我们可以提供通过实时媒体 SDK 的应用程序托管媒体选项。

### <a name="service-hosted-media"></a>服务承载媒体

自动程序可以管理工作流和卸载到 Microsoft 实时媒体平台的音频处理。 使用服务承载媒体，您必须实现和承载您 bot 多种选项。 请考虑使用一个可用的[Sdk](https://developer.microsoft.com/graph/code-samples-and-sdks)。 服务承载媒体自动程序可以实现作为无状态服务，如它不处理媒体本地。

| 方法                                                        | 说明                                             |
|:--------------------------------------------------------------|:--------------------------------------------------------|
| [PlayPrompt](../api/call-playprompt.md)                       | 向用户播放音频剪辑。                         |
| [Record](../api/call-record.md)                               | （可选） 播放提示和录制音频剪辑。      |
| [SubscribeToTone](../api/call-subscribetotone.md)             | 从用户订阅 DTMF 声音信号。                  |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md) | 取消任何处理已排队的媒体。             |

### <a name="application-hosted-media"></a>应用程序托管媒体

若要获取直接访问媒体 bot、 bot 需要访问媒体权限。 实时媒体库和状态 SDK 帮助您生成调用 bot 富实时媒体。 必须在 Windows 环境中承载应用程序托管的自动程序。 [应用程序托管的媒体示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples)说明如何生成 bot （包括云服务和服务结构） 的各种 Azure 平台中。

您可以使用[Microsoft Graph 呼叫 SDK](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html)简化创建自动程序。 SDK 提供功能来管理在内存中的资源的状态并提取自动程序开发人员的媒体堆栈中。

媒体 SDK 允许 bot 发送和接收音频、 视频和基于视频的屏幕共享内容。 基于视频的屏幕共享为视频信道建模。 Bot 可以订阅混合音频频道服务器和多个视频信道。 对于视频的通道，bot 已发送和接收视频编码的 H.264 流作为或已解码的原始框架可选择。

> **注意：** 您不可能使用 Microsoft.Graph.Calls.Media API 记录或否则保持从呼叫或您自动程序访问的会议的媒体内容。

## <a name="see-also"></a>另请参阅

[呼叫和联机会议 API 示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)

[已知问题](/graph/known-issues#calls-and-online-meetings)
