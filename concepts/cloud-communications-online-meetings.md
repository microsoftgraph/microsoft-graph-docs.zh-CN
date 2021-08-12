---
title: 使用云通信 API 创建或加入联机会议
description: 你可以灵活地创建将来或即时举行的会议
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 8e23438742f375914d87f5e5ed7289aaa2d202dd7b782a9345cba9121dbea33f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246456"
---
# <a name="use-the-cloud-communications-api-to-create-or-join-online-meetings"></a>使用云通信 API 创建或加入联机会议

联机会议提供指定特定详细信息（如会议主题以及所有与会者是谁）的能力。 还可以设置会议开始和结束的日期和时间。

联机会议提供了创建将来或瞬间召开会议的灵活性。 对于需要与会者立即注意的意外问题和其他事件，设置在会议创建后立即启动的会议是理想选择。

> **注意** 这组 API 允许灵活且更丰富的与Microsoft Teams或Skype集成;它不会在日历中更新或创建任何事件。 若要方便地将联机会议添加到日历Outlook，请使用日历 API。 有关详细信息，请参阅[在 Microsoft Graph 中选择 API 以创建和加入联机会议](choose-online-meeting-api.md)。

## <a name="create-an-online-meeting"></a>创建联机会议

创建联机会议时，将收到 [会议](/graph/api/resources/onlinemeeting) 坐标。 当参与者使用这些会议坐标加入会议时，将创建一个组呼叫。

当所有参与者离开组呼叫时，组呼叫将结束。 参与者在之后仍可使用相同的会议坐标重新加入会议，但此操作将创建另一个组呼叫。

>**注意：** 创建的会议不会显示在日历上。

## <a name="join-an-online-meeting"></a>加入联机会议
创建联机会议后，用户可以通过两种方式加入：

1. 通过浏览器，使用作为会议坐标的一部分 [返回的](/graph/api/resources/onlinemeeting)**joinWebURL。**

2. 通过[创建调用 API，](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media)这需要你提供会议坐标、 ([和](/graph/api/resources/organizermeetinginfo) [](/graph/api/resources/onlinemeeting) [chatInfo](/graph/api/resources/chatinfo)) 。

## <a name="see-also"></a>另请参阅

- [联机会议权限](./permissions-reference.md#online-meetings-permissions)
- [在 Microsoft Graph 中选择 API 以创建和加入联机会议](choose-online-meeting-api.md)