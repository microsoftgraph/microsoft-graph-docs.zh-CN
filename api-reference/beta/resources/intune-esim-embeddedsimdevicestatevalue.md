---
title: embeddedSIMDeviceStateValue 枚举类型
description: 描述嵌入的 SIM 激活代码的各种状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9bdc3250605de7db7a3778d64b5e743a415de4c0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145421"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>embeddedSIMDeviceStateValue 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述嵌入的 SIM 激活代码的各种状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notEvaluated|0|指明嵌入的 SIM 激活代码是免费的, 可以分配给设备。|
|failed|1|指定 Intune 服务无法将此配置文件传递给设备。|
|安装|双面|指定已将嵌入的 SIM 激活代码分配给设备, 并且设备正在安装令牌。|
|了|第三章|指定已在目标设备上成功安装嵌入的 SIM 激活代码。|
|删除|4|指定 Intune 服务正在尝试从设备中删除配置文件。|
|error|5|指定此配置文件存在错误。|
|deleted|型|指定将配置文件从设备中删除。|
|removedByUser|步|指定用户从设备中删除配置文件|




