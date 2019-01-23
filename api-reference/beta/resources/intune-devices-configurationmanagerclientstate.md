---
title: configurationManagerClientState 枚举类型
description: 配置管理器客户端状态
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 82f4b677001346f9bd32c1bc54bed6e7fbac253d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425783"
---
# <a name="configurationmanagerclientstate-enum-type"></a>configurationManagerClientState 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




