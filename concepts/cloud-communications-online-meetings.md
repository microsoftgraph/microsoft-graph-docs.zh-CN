---
title: 使用云通信 API 创建或加入联机会议
description: 使用 Microsoft Graph 中的云通信 API 创建或加入联机会议。 创建将来或即时发生的会议。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: 41d823f384cb9682c90be22982b3d676e5652912
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440969"
---
# <a name="create-or-join-online-meetings"></a>创建或加入联机会议

使用 Microsoft Graph 中的云通信 API 创建或加入联机会议。 联机会议提供指定特定详细信息的能力，例如会议的主题和所有与会者是谁。 还可以设置会议开始和结束的日期和时间。

联机会议可灵活地创建将来或即时举行的会议。 设置在创建会议后立即开始的会议的功能非常适合意外问题和其他需要与会者立即关注的事件。

> [!NOTE]
> 这组 API 允许与 Microsoft Teams 或 Skype 功能进行灵活和更丰富的集成;它不会更新或创建日历中的任何事件。 若要方便地将联机会议添加到 Outlook 日历，请使用日历 API。 有关详细信息，请参阅[在 Microsoft Graph 中选择 API 以创建和加入联机会议](choose-online-meeting-api.md)。

## <a name="create-an-online-meeting"></a>创建联机会议

创建联机会议时，你将收到会议的 [坐标](/graph/api/resources/onlinemeeting) 。 当参与者使用这些会议坐标加入会议时，将创建一个组调用。

当所有参与者离开组呼叫时，组调用将结束。 参与者仍然可以使用相同的会议坐标在之后重新加入会议，但这会创建另一个组调用。

> [!NOTE]
> 创建的会议不会显示在日历上。

## <a name="join-an-online-meeting"></a>加入联机会议

创建联机会议后，用户可以通过两种方式加入：

1. 通过浏览器，使用作为 [会议坐](/graph/api/resources/onlinemeeting)标的一部分返回的 **joinWebURL**。

2. 通过 [创建调用 API](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media)，需要提供 [会议坐标](/graph/api/resources/onlinemeeting)、 ([组织者meetinginfo](/graph/api/resources/organizermeetinginfo) 和 [chatInfo](/graph/api/resources/chatinfo)) 。

## <a name="see-also"></a>另请参阅

- [联机会议权限](./permissions-reference.md#online-meetings-permissions)
- [在 Microsoft Graph 中选择 API 以创建和加入联机会议](choose-online-meeting-api.md)
- [云通信 API 概述](cloud-communications-concept-overview.md)
