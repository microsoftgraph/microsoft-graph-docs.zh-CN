---
title: 使用 Microsoft Graph 通信 API
description: Microsoft Graph 通信 API 通过启用语音和视频功能，为应用和服务与用户的互动方式添加了新的维度。
author: VinodRavichandran
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 1f20413fe905cbbfb4e007386ff852476e00a79f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871079"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a>使用 Microsoft Graph 通信 API

Microsoft Graph 通信 API 通过在应用和服务中启用核心通信功能，为你或你的组织与其他用户交互的方式添加了新的维度。 可使用此 API 接听电话、创建和检索会议坐标。

可使用通信 API 构建服务应用程序（机器人），它们在通话中充当参与者，并代表用户创建和检索会议。
此 API 提供了通话功能，还可用于创建和检索联机会议。 可将服务应用程序（机器人）与此 API 搭配使用，其中机器人可在 VoIP 通话或 Microsoft Teams 会议中充当参与者等等。

## <a name="authorization"></a>授权

需要以下[权限](https://docs.microsoft.com/graph/permissions-reference#calls-permissions) 之一才能访问通信 API。 需要由管理员授予这些权限。

| 方案                 | 权限                                  |
|:------------------------------------|:---------------------------------------------|
| 通话                 | Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All |
| 会议                 | OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All |

## <a name="common-use-cases"></a>常见用例

下表列出了通信 API 的一些常见用例。

| 用例                         | REST 资源                                 | 另请参阅  |
|:------------------------------------|:---------------------------------------------|:----------|
| 创建并键入一对一通话和群组通话   | [通话](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0)| [通话方法](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0#methods)| 
|IVR 通话   |     | [IVR 方法](https://docs.microsoft.com/graph/api/resources/calls-api-ivr-overview?view=graph-rest-v1.0)
| 通话控制（参与者） | [参与者](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-v1.0)   ||
|会议|[onlineMeeting](https://docs.microsoft.comgraph/api/resources/onlinemeeting?view=graph-rest-v1.0)| [会议方法](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#methods)|

## <a name="common-properties"></a>通用属性

| 资源                | 属性                             |
|:------------------------------------|:---------------------------------------------|
| 通话                               | [通话属性](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0#properties)  |
| 参与者                         | [参与者属性](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-v1.0#properties) |
| onlineMeeting                            | [onlineMeeting 属性](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#properties)                     |

## <a name="see-also"></a>另请参阅

- [通信 API 示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [通信信号 SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)
- [通信媒体 SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media)
