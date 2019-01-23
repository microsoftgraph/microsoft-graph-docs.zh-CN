---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等方通讯组的传递优化模式
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5565965f9ba9395d7cd07b2935e6772478e0bb50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406883"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对等方通讯组的传递优化模式

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|用户定制|0|允许用户设置。|
|为 httpOnly|1|HTTP 仅，没有对等|
|httpWithPeeringNat|2|与同一个网络地址转换器后面对等的 OS 默认 – Http 混合|
|httpWithPeeringPrivateGroup|3|HTTP 与跨专用组对等混合|
|httpWithInternetPeering|4|与 Internet 对等混合的 HTTP|
|simpleDownload|99|与没有对等的简单 download 模式|
|bypassMode|100|绕过模式。 不使用传递优化并改用位|




