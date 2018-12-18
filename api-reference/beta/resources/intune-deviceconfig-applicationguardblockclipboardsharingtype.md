---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: tfitzmac
ms.openlocfilehash: d55945c0e229801bab9a338a475e6ef6fd5e8b02
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311506"
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





