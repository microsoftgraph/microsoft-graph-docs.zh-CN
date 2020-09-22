---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 209cacfad96a4523cce3a6125652dc86f61227d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994202"
---
# <a name="emailsyncschedule-enum-type"></a>emailSyncSchedule 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

电子邮件同步计划的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|用户定义，默认值，无意向。|
|asMessagesArrive|1 |邮件到达时同步。|
|手动|2 |手动同步。|
|fifteenMinutes|第三章|每十五分钟同步一次。|
|thirtyMinutes|4 |每三十分钟同步一次。|
|sixtyMinutes|5 |每60分钟同步一次。|
|basedOnMyUsage|6 |根据我的使用情况进行同步。|






