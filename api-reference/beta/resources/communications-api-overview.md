---
title: 使用 Microsoft Graph 中的云通信 API
description: Microsoft Graph 云通信 API 通过启用语音和视频功能，为应用和服务与用户的互动方式添加了新的维度。
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
ms.localizationpriority: high
ms.openlocfilehash: 2b6748d9e2d8f3a0720053083daa33c751554150
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668060"
---
# <a name="working-with-the-cloud-communications-api-in-microsoft-graph"></a>使用 Microsoft Graph 中的云通信 API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph 云通信 API 通过在应用和服务中启用核心通信功能，为你或你的组织与其他用户交互的方式添加了新的维度。 可使用此 API 接听电话、创建和检索会议坐标和查看用户的状态。

可使用云通信 API 构建服务应用程序（机器人），它们在通话中充当参与者，代表用户创建和检索会议并检查出席状态和活动。
此 API 提供了通话功能，还可用于创建和检索联机会议。 可将服务应用程序（机器人）与此 API 搭配使用，其中机器人可在 VoIP 通话或 Microsoft Teams 会议中充当参与者等等。

## <a name="authorization"></a>授权

需要以下[权限](/graph/permissions-reference#calls-permissions)之一才能访问云通信 API。 需要由管理员授予这些权限。

| 方案                 | 权限                                  |
|:------------------------------------|:---------------------------------------------|
| 通话                 | Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All |
| 会议                 | OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All |
| 状态                 | 状态.阅读，状态.阅读.全部 |
| 通话记录             | CallRecords.Read.All |

## <a name="common-use-cases"></a>常见用例

下表列出了云通信 API 的一些常见用例。

| 用例                         | REST 资源                                 | 另请参阅  |
|:------------------------------------|:---------------------------------------------|:----------|
| 创建并键入一对一通话和群组通话   | [通话](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true&preserve-view=true)| [通话方法](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true#methods&preserve-view=true)|
|IVR 通话   |     | [IVR 方法](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta?&preserve-view=true&preserve-view=true)
| 通话控制（参与者） | [参与者](/graph/api/resources/participant?view=graph-rest-beta&preserve-view=true&preserve-view=true)   ||
|会议|[onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true&preserve-view=true)| [会议方法](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true#methods&preserve-view=true)|
|状态 | [状态](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true) | [出席方式](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true#methods) |
| 检索通话记录 | [callRecord](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta&preserve-view=true&preserve-view=true) | [Webhook 订阅](/graph/api/resources/webhooks?view=graph-rest-beta&preserve-view=true&preserve-view=true) |

## <a name="common-properties"></a>通用属性

| 资源                | 属性                             |
|:------------------------------------|:---------------------------------------------|
| 通话                               | [通话属性](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true#properties&preserve-view=true)  |
| 参与者                         | [参与者属性](/graph/api/resources/participant?view=graph-rest-beta?view=graph-rest-v1.0&preserve-view=true#properties&preserve-view=true) |
| onlineMeeting                            | [onlineMeeting 属性](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true#properties&preserve-view=true)                     |
| 状态 | [状态属性](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true#properties) |
| callRecord | [callRecord 属性](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta&preserve-view=true#properties) |

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="see-also"></a>另请参阅

- [云通信 API 示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [通信信号 SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls/1.0.0-prerelease.494)
- [通信媒体 SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media/1.0.0-prerelease.494)


