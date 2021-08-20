---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8ba1c5a506e5eb8eb7831794c47d73f0c7166fc876ef40acb1b023f7cd0a3860
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54165768"
---
# <a name="emailsyncschedule-enum-type"></a>emailSyncSchedule 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

电子邮件同步计划的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|用户定义，默认值，无意图。|
|asMessagesArrive|1 |在消息到达时同步。|
|手动|2 |手动同步。|
|fifteenMinutes|3 |每十五分钟同步一次。|
|thirtyMinutes|4 |每隔 30 分钟同步一次。|
|将minutes|5 |每隔 10 分钟同步一次。|
|basedOnMyUsage|6 |根据我的使用情况进行同步。|




