---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等方通讯组的传递优化模式
author: tfitzmac
ms.openlocfilehash: b23bdc80bd8b1fb151f9e138e1a1802140455c4e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333479"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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





