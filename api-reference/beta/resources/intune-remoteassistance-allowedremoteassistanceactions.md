---
title: allowedRemoteAssistanceActions 枚举类型
description: Flags 枚举，指示帮助程序是否可以建立视图屏幕、使用设备或共享者进行完全控制以及提升远程协助操作
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d002a27a95edc28c35dee2aeacf5e0a5a759fe5
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265551"
---
# <a name="allowedremoteassistanceactions-enum-type"></a>allowedRemoteAssistanceActions 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Flags 枚举，指示帮助程序是否可以与设备或共享者建立"查看屏幕"、"完全控制"和"提升"远程协助操作

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|viewScreen|1 |帮助程序可以查看共享者设备的屏幕|
|takeFullControl|2 |帮助程序可以完全控制共享者的设备|
|elevation|4 |帮助程序可以使用提升的权限完全控制共享者的设备|




