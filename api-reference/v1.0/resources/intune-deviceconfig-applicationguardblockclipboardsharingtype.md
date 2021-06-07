---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: applicationGuardBlockClipboardSharingType 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a70f654c283a32db4e89ccc1b3991ffba49fc89e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755936"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a>applicationGuardBlockClipboardSharingType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

applicationGuardBlockClipboardSharingType 的可能值

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notConfigured|0|未配置|
|blockBoth|1|阻止剪贴板从主机共享到容器以及从容器共享数据到主机|
|blockHostToContainer|2|阻止剪贴板将数据从主机共享到容器|
|blockContainerToHost|3|阻止剪贴板将数据从容器共享到主机|
|blockNone|4 |阻止剪贴板从主机共享到容器，也不从容器共享数据到主机|




