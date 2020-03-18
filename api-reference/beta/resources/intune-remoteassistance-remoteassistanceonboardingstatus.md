---
title: remoteAssistanceOnboardingStatus 枚举类型
description: 当前 TeamViewer 连接器状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 68e5a8bff7f1753540a2716a00fd9148e188d7ea
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772935"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>remoteAssistanceOnboardingStatus 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

当前 TeamViewer 连接器状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notOnboarded|0|当没有已配置或活动的活动的 TeamViewer 连接器时报告的状态|
|加入|1|系统启动 TeamViewer 连接时报告的状态，但该服务尚未完成连接器的确认|
|载入|双面|系统使用 TeamViewer 成功交换帐户信息并可以立即启动与客户端的远程协助会话时报告的状态|



