---
title: configurationManagerClientState 枚举类型
description: 配置管理器客户端状态
ms.openlocfilehash: c76fc33fee0fd5f6f5782f77d988535ec851cc86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047164"
---
# <a name="configurationmanagerclientstate-enum-type"></a>configurationManagerClientState 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

配置管理器客户端状态
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|配置管理器代理早于 1806年或未安装或此设备超过 30 天未签入 Intune。|
|安装|1|配置管理器代理已安装，但可能不出现在配置管理器控制台尚未。 等待几个小时才能刷新。|
|正常运行|7|此设备就能够成功签入的配置管理器服务。|
|installFailed|8|配置管理器代理安装失败。|
|updateFailed|11|从 x 版本到版本的配置管理器代理 y 的更新失败。 |
|communicationError|19|配置管理器代理能够找到配置管理器服务在过去但现在不再能够。 |





