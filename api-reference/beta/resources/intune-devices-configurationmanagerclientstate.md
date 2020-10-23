---
title: configurationManagerClientState 枚举类型
description: 配置管理器客户端状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: de8f2af7c6d35b28154f00a4eac3bb20a4bdf64d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690229"
---
# <a name="configurationmanagerclientstate-enum-type"></a>configurationManagerClientState 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

配置管理器客户端状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|配置管理器代理早于1806或未安装，或者此设备未签入 Intune 的30天。|
|了|1|配置管理器代理已安装，但可能尚未在 configuration manager 控制台中显示。 请等待几小时，让其刷新。|
|运转|7 |此设备能够成功签入 configuration manager 服务。|
|installFailed|8 |配置管理器代理安装失败。|
|updateFailed|11x17|从版本 x 更新到配置管理器代理版本 y 的更新失败。 |
|communicationError|合|Configuration manager 代理在过去能够到达 configuration manager 服务，但现在无法再访问。 |





