---
title: 使用 Microsoft Graph 中的呼叫和在线会议 API
description: Microsoft Graph 呼叫和在线会议 API 通过启用语音和视频功能，为应用程序和服务与用户的互动方式添加了新的维度。 该 API 可让你创建呼叫并接收来自 Microsoft Teams 中的用户和应用程序的呼叫。 你可以使用这些 API 构建可在呼叫或会议中充当参与者的服务应用程序（机器人）。
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: conceptualPageType
ms.openlocfilehash: dea588035e2f19361a36450bb49b4c5b2d9391b5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013008"
---
# <a name="working-with-the-calls-and-online-meetings-api-in-microsoft-graph"></a>使用 Microsoft Graph 中的呼叫和在线会议 API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph 呼叫和在线会议 API 通过启用语音和视频功能，为应用程序和服务与用户的互动方式添加了新的维度。 该 API 可让你创建呼叫并接收来自 Microsoft Teams 中的用户和应用程序的呼叫。 你可以使用这些 API 构建可在呼叫或会议中充当参与者的服务应用程序（机器人）。

## <a name="call-types"></a>呼叫类型

呼叫分为对等呼叫和多方呼叫。 用户可以向机器人发起对等呼叫，也可以邀请机器人加入现有的多方会议。 当用户邀请机器人进行对等呼叫时，无需任何权限。 若要让机器人参与多方呼叫，机器人需要获得租户管理员的许可才能加入群组通话。

![显示对等呼叫和多方呼叫的图像](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/call-types.png)

如果要让机器人创建呼叫，它需要具有发起呼叫或发起群组通话的权限。 机器人可以选择创建对等呼叫或多方呼叫。

- 对于对等呼叫，机器人只需要指定一个目标，而无需指定会议坐标。 
- 如果机器人向多名参与者发起呼叫，则会在幕后设置临时会议，并且每个人都可加入该会议。 如果指定了会议坐标，则即使只有一个目标，也会设置多方呼叫。

呼叫可能会以对等的方式开始，并升级为多方。 系统将自动设置会议，并且媒体将重定向到会议。 如果机器人具有发起群组通话的权限，则它可以通过邀请其他人来发起升级。 如果升级是由另一名参与者发起的并且机器人没有加入群组通话的权限，那么将从通话中删除该机器人。

> **重要说明：** 如果将呼叫从对等升级为多方，则并非所有多方呼叫功能都可用。 具体而言，机器人无法接收名单更新。

## <a name="signaling"></a>信号

### <a name="incoming-call"></a>传入呼叫

若要接收传入呼叫，你需要注册呼叫机器人。 当机器人接收传入通知时，它包含以下选项。

| 方法                              | 说明                                  |
|:------------------------------------|:---------------------------------------------|
| [应答](../api/call-answer.md)     | 应答传入呼叫。                    |
| [拒绝](../api/call-reject.md)     | 拒绝并挂断呼叫。                  |
| [重定向](../api/call-redirect.md) | 重定向呼叫。                           |

机器人可以将呼叫重定向到其他用户或机器人。 机器人还可以将它重定向到用户的语音邮件。

![显示机器人将呼叫重定向到语音邮件的图像](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/call-handling.png)

> **重要说明：** 目前不支持向 PSTN 进行重定向或出站呼叫。

### <a name="in-call"></a>通话中

机器人操作在呼叫对象上可用。 这会影响机器人作为参与者加入呼叫。

| 方法                                                            | 说明                                  |
|:------------------------------------------------------------------|:---------------------------------------------|
| [静音](../api/call-mute.md)                                       | 在呼叫中将自己设为静音。                       |
| [取消静音](../api/call-unmute.md)                                   | 在呼叫中将自己取消静音。                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | 在名单中更新自己的元数据。          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) | 在呼叫中开始和停止共享屏幕。   |

若要与呼叫中的其他参与者进行互动，请使用参与者对象。

| 方法                                                            | 说明                                  |
|:------------------------------------------------------------------|:---------------------------------------------|
| [列出参与者](../api/call-list-participants.md)             | 获取参与者对象集合。         |
| [邀请参与者](../api/participant-invite.md)               | 邀请参与者加入活动呼叫。      |
| [将所有参与者设为静音](../api/participant-muteall.md)            | 将呼叫中的所有参与者设为静音。           |

## <a name="media"></a>媒体

通过 Microsoft 实时媒体平台来管理媒体处理。 实时媒体平台可帮助机器人参与 Microsoft Teams 音频/视频通话和会议。 它允许实时机器人参与对等呼叫和多方呼叫。

当机器人接听来电或加入新呼叫或现有呼叫时，需要告诉实时媒体平台如何处理媒体。 如果要构建互动语音响应 (IVR) 系统，则可以将昂贵的音频处理卸载到 Microsoft 服务托管的媒体组件。 如果机器人需要直接访问媒体流，我们会通过实时媒体 SDK 提供应用程序托管的媒体选项。

### <a name="service-hosted-media"></a>服务托管的媒体

机器人可以管理工作流并将音频处理卸载到 Microsoft 实时媒体平台。 对于服务托管的媒体，你可以通过多个选项来实施和托管机器人。 请考虑使用其中一个可用的 [SDK](https://developer.microsoft.com/graph/code-samples-and-sdks)。 服务托管的媒体机器人可以作为无状态服务进行实施，因为它不在本地处理媒体。

| 方法                                                        | 说明                                             |
|:--------------------------------------------------------------|:--------------------------------------------------------|
| [PlayPrompt](../api/call-playprompt.md)                       | 向用户播放音频剪辑。                         |
| [录制](../api/call-record.md)                               | （可选）播放提示并录制音频剪辑。      |
| [SubscribeToTone](../api/call-subscribetotone.md)             | 订阅用户的 DTMF 音。                  |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md) | 取消已排队的所有媒体处理。             |

### <a name="application-hosted-media"></a>应用程序托管的媒体

若要让机器人直接访问媒体，该机器人需要具有访问媒体的权限。 实时媒体库和有状态 SDK 可帮助你构建各种实时媒体呼叫机器人。 必须在 Windows 环境中托管应用程序托管的机器人。 [应用程序托管的媒体示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples)显示了如何在各种 Azure 平台（包括云服务和 Service Fabric）中构建机器人。

你可以使用 [Microsoft Graph 呼叫 SDK](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html) 简化机器人的创建过程。 该 SDK 提供了用于管理内存中的资源状态和引入机器人开发人员媒体堆栈的功能。

媒体 SDK 允许机器人发送和接收音频、视频以及基于视频的屏幕共享内容。 基于视频的屏幕共享将作为视频频道进行建模。 机器人可以订阅混合音频频道和多个视频频道。 对于视频频道，机器人可以选择以编码的 H.264 流或解码的原始帧发送和接收视频。

> **注释：** 请勿使用 Microsoft.Graph.Calls.Media API 来记录或以其他方式保留机器人访问的通话或会议中的媒体内容。

## <a name="see-also"></a>另请参阅

[呼叫和在线会议 API 示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)

[已知问题](/graph/known-issues#calls-and-online-meetings)
