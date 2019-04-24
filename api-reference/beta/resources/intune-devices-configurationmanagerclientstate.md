---
title: configurationManagerClientState 枚举类型
description: 配置管理器客户端状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f6231ecebf407172f2c7178a130d90200868292
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454242"
---
# <a name="configurationmanagerclientstate-enum-type"></a>configurationManagerClientState 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

配置管理器客户端状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|配置管理器代理早于1806或未安装, 或者此设备未签入 Intune 的30天。|
|了|1|配置管理器代理已安装, 但可能尚未在 configuration manager 控制台中显示。 请等待几小时, 让其刷新。|
|运转|步|此设备能够成功签入 configuration manager 服务。|
|installFailed|utf-8|配置管理器代理安装失败。|
|updateFailed|11x17|从版本 x 更新到配置管理器代理版本 y 的更新失败。 |
|communicationError|合|configuration manager 代理在过去能够到达 configuration manager 服务, 但现在无法再访问。 |





