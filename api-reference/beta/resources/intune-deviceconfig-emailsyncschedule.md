---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f2d7d9d4918946b3683bce5f118fa9a04edf7afe
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791798"
---
# <a name="emailsyncschedule-enum-type"></a>emailSyncSchedule 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

电子邮件同步计划的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|用户定义，默认值，无意向。|
|asMessagesArrive|1|邮件到达时同步。|
|手动|双面|手动同步。|
|fifteenMinutes|第三章|每十五分钟同步一次。|
|thirtyMinutes|4 |每三十分钟同步一次。|
|sixtyMinutes|5 |每60分钟同步一次。|
|basedOnMyUsage|6 |根据我的使用情况进行同步。|



