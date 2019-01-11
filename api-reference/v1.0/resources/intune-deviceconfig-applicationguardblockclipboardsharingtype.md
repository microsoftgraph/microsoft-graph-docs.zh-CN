---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6fe418aa1f91c0e65770b797781dda9e29803d86
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865973"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a>applicationGuardBlockClipboardSharingType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

ApplicationGuardBlockClipboardSharingType 的可能值
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notConfigured|0|未配置|
|blockBoth|1|阻止剪贴板共享数据从主机到容器和容器迁移到主机|
|blockHostToContainer|2|阻止剪贴板共享数据从主机到容器|
|blockContainerToHost|3|阻止剪贴板共享数据从容器到主机|
|blockNone|4|共享数据从主机到容器和从容器迁移到主机都不阻止剪贴板|



