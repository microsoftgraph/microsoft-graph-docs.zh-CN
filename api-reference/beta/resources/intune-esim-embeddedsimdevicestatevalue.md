---
title: embeddedSIMDeviceStateValue 枚举类型
description: 介绍为嵌入 SIM 激活代码的各种状态。
ms.openlocfilehash: c0b1cffedcae18dab4c1d23a2691cafa8709c0ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042587"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>embeddedSIMDeviceStateValue 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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





