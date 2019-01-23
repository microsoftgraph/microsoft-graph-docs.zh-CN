---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8285b9a34e208b86b7c53c38e6aa015fd8c37560
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425181"
---
# <a name="emailsyncschedule-enum-type"></a>emailSyncSchedule 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




