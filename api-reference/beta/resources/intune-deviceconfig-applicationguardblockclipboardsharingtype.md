---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 91c2bceba0d4ffda030266d0f5617ce18ab29f68
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49216379"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a>applicationGuardBlockClipboardSharingType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ApplicationGuardBlockClipboardSharingType 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置|
|blockBoth|1|阻止剪贴板将数据从主机共享到容器，并将容器从容器共享到主机|
|blockHostToContainer|双面|阻止剪贴板将数据从主机共享到容器|
|blockContainerToHost|第三章|阻止剪贴板将数据从容器共享到主机|
|blockNone|4 |阻止剪贴板将数据从主机共享到容器，也不将其从容器共享到主机|




