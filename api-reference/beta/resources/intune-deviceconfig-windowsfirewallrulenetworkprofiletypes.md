---
title: windowsFirewallRuleNetworkProfileTypes 枚举类型
description: 表示哪些网络配置文件类型适用于防火墙规则的标志。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9e46fccf175483090bc78ae0c070112c7e3f18e9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49215329"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a>windowsFirewallRuleNetworkProfileTypes 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示哪些网络配置文件类型适用于防火墙规则的标志。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未设置任何标志。|
|domain|1|连接到域的网络的配置文件。|
|private|双面|专用网络的配置文件。|
|公开|4 |公用网络的配置文件。|




