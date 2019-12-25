---
title: 联机会议概述
description: 你可以灵活地创建将来或即时使用的会议
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: bd85c3be66890d4763e2c2b1910ee7049573d446
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871569"
---
# <a name="online-meetings-overview"></a>联机会议概述

联机会议提供了指定特定详细信息（如会议主题和所有与会者）的功能。 您还可以设置会议开始和结束的日期和时间。

在线会议提供了创建将来或即时召开会议的灵活性。 设置在创建后立即启动的会议的功能对于需要立即关注与会者的意外问题和其他事件来说是理想之选。

## <a name="create-an-online-meeting"></a>创建联机会议

创建联机会议时，将接收会议的[坐标](/graph/api/resources/onlinemeeting)。 当参与者使用这些会议坐标加入会议时，将会创建一个组呼叫。

当所有参与者都离开组呼叫时，组呼叫将结束。 参与者仍可以使用相同的会议坐标在随后重新加入会议，但这将创建另一个组呼叫。

>**注意：** 创建的会议不会显示在日历上。

## <a name="join-an-online-meeting"></a>加入联机会议
在创建联机会议之后，用户可以通过以下两种方式加入：

1. 通过浏览器，使用作为[会议坐标](/graph/api/resources/onlinemeeting)一部分返回的**joinURL** 。

2. 通过[创建调用 API](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media)，它需要您提供[会议坐标](/graph/api/resources/onlinemeeting)（[organizermeetinginfo](/graph/api/resources/organizermeetinginfo)和[chatInfo](/graph/api/resources/chatinfo)）。

## <a name="see-also"></a>另请参阅

- [联机会议权限](/graph/permissions-reference#online-meetings-permissions)
