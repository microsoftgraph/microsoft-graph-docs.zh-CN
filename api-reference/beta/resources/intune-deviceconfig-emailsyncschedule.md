---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
ms.openlocfilehash: 48c5d433815d5f27d018d97ac479641146754669
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041632"
---
# <a name="emailsyncschedule-enum-type"></a>emailSyncSchedule 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

电子邮件同步计划的可能值。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|用户定制|0|用户定义，默认值、 没有用途。|
|asMessagesArrive|1|当消息到达同步。|
|手动|2|手动同步。|
|fifteenMinutes|3|同步每 15 分钟。|
|thirtyMinutes|4|同步每 30 分钟。|
|sixtyMinutes|5|同步每隔 60 分钟。|
|basedOnMyUsage|6|根据我使用情况的同步。|





