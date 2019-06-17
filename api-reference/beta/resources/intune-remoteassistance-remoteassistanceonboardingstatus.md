---
title: remoteAssistanceOnboardingStatus 枚举类型
description: 当前 TeamViewer 连接器状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12a127b053482d87a17cb8c3e5ca4a7191ce32aa
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996272"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>remoteAssistanceOnboardingStatus 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

当前 TeamViewer 连接器状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notOnboarded|0|当没有已配置或活动的活动的 TeamViewer 连接器时报告的状态|
|加入|1|系统启动 TeamViewer 连接时报告的状态, 但该服务尚未完成连接器的确认|
|载入|双面|系统使用 TeamViewer 成功交换帐户信息并可以立即启动与客户端的远程协助会话时报告的状态|





