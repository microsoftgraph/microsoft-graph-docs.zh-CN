---
title: remoteAssistanceOnboardingStatus 枚举类型
description: 当前的 TeamViewer 连接器状态
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ea059025920da62824d816062fe60c03d6b5938d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039481"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>remoteAssistanceOnboardingStatus 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

当前的 TeamViewer 连接器状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notOnboarded|0|未配置或处于活动状态的 TeamViewer 连接器时报告的状态|
|载入|1|当系统启动 TeamViewer 连接，但服务尚未完成连接器确认时报告的状态|
|已载入|2|当系统已成功与 TeamViewer 交换帐户信息，并且现在可以与客户端启动远程协助会话时报告的状态|



