---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
ms.openlocfilehash: e0e05001e4f3cedc2893fc6b2006f5b5b5d74db6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045892"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a>applicationGuardBlockClipboardSharingType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

ApplicationGuardBlockClipboardSharingType 的可能值
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置|
|blockBoth|1|阻止剪贴板共享数据从主机到容器和容器迁移到主机|
|blockHostToContainer|2|阻止剪贴板共享数据从主机到容器|
|blockContainerToHost|3|阻止剪贴板共享数据从容器到主机|
|blockNone|4|共享数据从主机到容器和从容器迁移到主机都不阻止剪贴板|





