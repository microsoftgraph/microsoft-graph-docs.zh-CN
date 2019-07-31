---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 14b73fc4cfbf9cf53bdab4c2841403cac4077fa2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001423"
---
# <a name="emailsyncschedule-enum-type"></a>emailSyncSchedule 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

电子邮件同步计划的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|用户定义, 默认值, 无意向。|
|asMessagesArrive|1|邮件到达时同步。|
|手动|双面|手动同步。|
|fifteenMinutes|第三章|每十五分钟同步一次。|
|thirtyMinutes|4|每三十分钟同步一次。|
|sixtyMinutes|5|每60分钟同步一次。|
|basedOnMyUsage|型|根据我的使用情况进行同步。|





