---
title: remoteAssistanceOnboardingStatus 枚举类型
description: 当前 TeamViewer 连接器状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ccb04964c7608c24ec8822bac7832aaf77bdfd7f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287786"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>remoteAssistanceOnboardingStatus 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

当前 TeamViewer 连接器状态

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notOnboarded|0|当没有已配置或活动的活动的 TeamViewer 连接器时报告的状态|
|加入|1|系统启动 TeamViewer 连接时报告的状态，但该服务尚未完成连接器的确认|
|载入|双面|系统使用 TeamViewer 成功交换帐户信息并可以立即启动与客户端的远程协助会话时报告的状态|




