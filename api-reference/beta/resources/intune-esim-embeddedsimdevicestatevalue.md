---
title: embeddedSIMDeviceStateValue 枚举类型
description: 介绍为嵌入 SIM 激活代码的各种状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2da255ef2d0cf192dd09a6351bbd337f3cd9b5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421324"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>embeddedSIMDeviceStateValue 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

介绍为嵌入 SIM 激活代码的各种状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notEvaluated|0|指定嵌入的 SIM 激活代码可用，并且可以分配给设备。|
|failed|1|指定 Intune 服务未能向设备提供此配置文件。|
|安装|2|指定的嵌入式的 SIM 激活代码已分配给设备和设备安装令牌。|
|安装|3|指定已成功目标设备上安装的嵌入的 SIM 激活代码。|
|删除|4|指定 Intune 服务尝试从设备中删除配置文件。|
|error|5|指定存在与此配置文件的错误。|
|deleted|6|指定从设备中删除配置文件。|
|removedByUser|7|指定从设备删除配置文件的用户|




